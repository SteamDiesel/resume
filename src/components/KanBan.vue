<template>
	<div class="flex">
		<div
			v-for="(stage, index) in sortedDeals"
			:key="index"
			@dragenter.prevent
			@dragover.prevent
			@drop="dragDrop"
			class="bg-grey-300 border border-2 border-grey-400 rounded-lg p-4 h-64 w-full m-10"
			:id="stage.title"
		>
			<div
				v-for="(deal, index) in stage.deals"
				:key="index"
				draggable="true"
				@dragstart="startDrag"
				:id="deal.uuid"
				class="border border-orange-300 border-0 p-4 my-2"
			>
				{{ deal.title }} {{ deal.uuid }}
			</div>
		</div>
	</div>
</template>

<script>
	export default {
		components: {},
		data() {
			return {
				deals: [
					{ title: "Dean", stage: "stage 1", uuid: "uuid687322" },
					{ title: "Eric", stage: "stage 2", uuid: "uuid312988" },
					{ title: "Diego", stage: "stage 3", uuid: "uuid888955" },
					{ title: "Mike", stage: "stage 1", uuid: "uuid519615" },
					{ title: "Ian", stage: "stage 1", uuid: "uuid519656" },
					{ title: "Chris", stage: "stage 1", uuid: "uuid519645" },
					{ title: "Damien", stage: "stage 1", uuid: "uuid519634" },
					{ title: "Poe", stage: "stage 1", uuid: "uuid519623" },
				],
				deal_id: "",

				stages: ["stage 1", "stage 2", "stage 3", "stage 4"],
			};
		},
		computed: {
			sortedDeals() {
				console.log("sorting deals ...");
				var deals = [];
				this.stages.forEach((stage) => {
					deals.push({
						title: stage,
						deals: this.deals.filter((item) => {
							return item.stage == stage;
						}),
					});
				});
				return deals;
			},
		},
		methods: {
			// Parent element (column) functions
			// make parent element @draggable
			// the e.target.id for these functions point to the parent element. so any attributes given to the parent element can be accessed
			// @dragend
			// endDrag(e) {
			// 	console.log("end " + e.target.id); // end target is the child
			// 	setTimeout(() => {
			// 		e.target.style.display = "block";
			// 	});
			// },
			// // @dragover.stop (stop will let the 'drop' event fire)
			// dragOver(e) {
			// 	e.preventDefault();
			// 	// console.log("dragover ");
			// },
			// //  @dragenter
			// dragEnter(e) {
			// 	this.destination_stage = e.target.id;
			// 	console.log("dragEnter " + e.target.id);
			// },
			// // @dragleave
			// dragLeave(e) {
			// 	console.log("dragLeave " + e.target.id);
			// },
			dragDrop(e) {
				const deal_id = e.dataTransfer.getData("deal_id");
				// const deal = document.getElementById(deal_id);
				var deal_index = this.deals.findIndex((deal) => {
					return deal.uuid == deal_id;
				});
				// console.log(deal_index);
				this.deals[deal_index].stage = e.target.id;
				// deal.style.display = "block";

				// console.log("drop " + e.target.id);
			},

			// Child element (card) functions
			// @dragstart
			startDrag(e) {
				// console.log("startDrag " + e.target.id);
				this.deal_id = e.target.id;
				e.dataTransfer.setData("deal_id", e.target.id);
				setTimeout(() => {
					// This function is important to trigger something. note sure what though...
					// e.target.style.display = "none";
				});
			},

			updateDealStage() {},
		},
		mounted() {},
	};
</script>

<style></style>
