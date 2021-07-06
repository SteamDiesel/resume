<template>
	<div id="app">
		<div class="print:hidden flex flex-col p-14">
			<select
				v-model="application"
				class="form-input text-center border-2 bg-gray-100"
			>
				<!-- inline object literal -->
				<option
					v-for="(app, index) in applications"
					:value="app"
					:key="index"
					:id="index"
					>{{ app.employer }}</option
				>
			</select>

			<button
				class="bg-blue-300 border border-blue-400 rounded-sm w-32 mt-2"
				@click.prevent="newApp"
			>
				new
			</button>
		</div>

		<Cover :name="name">
			<template v-slot:position>
				<input
					class="text-2xl font-semibold text-orange-600 w-full p-1"
					type="text"
					name=""
					id="applicationposition"
					v-model="application.position"
					@keyup="saveApps"
				/>
			</template>
			<template v-slot:employer>
				<input
					class="text-lg font-semibold text-gray-600 mb-14 w-full p-1"
					type="text"
					name=""
					id="applicationemployer"
					v-model="application.employer"
					@keyup="saveApps"
				/>
			</template>
			<template v-slot:body>
				<div>
					<textarea
						v-model="application.coverbody"
						@keyup="saveApps"
						name=""
						id="coverbodyfield"
						rows="35"
						class="w-full p-1 text-md"
					></textarea>
				</div>
			</template>
		</Cover>

		<Resume :name="name" :position="application.position" />
	</div>
</template>

<script>
	import Cover from "./components/Cover.vue";
	import Resume from "./components/Resume.vue";

	export default {
		name: "App",
		components: {
			Cover,
			Resume,
		},
		data() {
			return {
				saved: true,
				edit: true,
				name: "Jason Law",
				application: {},
				applications: [
					{
						employer: "Blank Employer 1",
						position: "Position",
						coverbody: "Dear... \n \n\nSincerely,\n\n",
					},
					{
						employer: "Blank Employer 2",
						position: "Position",
						coverbody: "Dear... \n \n\nSincerely,\n\n",
					},
				],
			};
		},
		methods: {
			newApp() {
				var app = {
					employer: "Employer",
					position: "Position",
					coverbody: "Dear... \n\n\nSincerely, \n\n",
				};
				this.applications.push(app);

				this.application = app;
			},
			saveApps() {
				try {
					localStorage.setItem(
						"applications",
						JSON.stringify(this.applications)
					);
					window.console.log("Saved to local browser storage.");
				} catch {
					window.console.log(
						"Unable to save applications to local storage."
					);
					alert("Unable to save applications to local storage.");
				}
			},
			initialize() {
				try {
					this.applications = JSON.parse(
						localStorage.getItem("applications")
					);
					window.console.log(
						"Retrieved Applications data from local storage."
					);
				} catch {
					window.console.log(
						"Unable to retrieve Applications data from local storage."
					);
				}
			},
		},
		mounted() {
			this.initialize();
		},
	};
</script>

<style></style>
