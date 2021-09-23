<template>
	<div class="bg-green-500">
		<div
			class="py-24 flex items-center justify-center bg-gray-50 py-12 px-4 sm:px-6 lg:px-8"
		>
			<div class="max-w-md w-full space-y-8">
				<input type="hidden" name="remember" value="true" />
				<div class="rounded-md shadow-sm -space-y-px">
					<div>
						<label for="name" class="sr-only">Name</label>
						<input
							v-model="user.name"
							id="name"
							name="name"
							type="text"
							class="appearance-none rounded-none relative block w-full px-3 py-2 border border-gray-300 placeholder-gray-500 text-gray-900 rounded-t-md focus:outline-none focus:ring-indigo-500 focus:border-indigo-500 focus:z-10 sm:text-sm"
							placeholder="Name"
						/>
					</div>
					<div>
						<label for="email-address" class="sr-only"
							>Email address</label
						>
						<input
							v-model="user.email"
							id="email-address"
							name="email"
							type="email"
							autocomplete="email"
							class="appearance-none rounded-none relative block w-full px-3 py-2 border border-gray-300 placeholder-gray-500 text-gray-900 rounded-t-md focus:outline-none focus:ring-indigo-500 focus:border-indigo-500 focus:z-10 sm:text-sm"
							placeholder="Email address"
						/>
					</div>
					<div>
						<label for="password" class="sr-only">Password</label>
						<input
							v-model="user.password"
							id="password"
							name="password"
							type="password"
							autocomplete="current-password"
							class="appearance-none rounded-none relative block w-full px-3 py-2 border border-gray-300 placeholder-gray-500 text-gray-900 rounded-b-md focus:outline-none focus:ring-indigo-500 focus:border-indigo-500 focus:z-10 sm:text-sm"
							placeholder="Password"
						/>
					</div>
					<div>uuid {{ user.uuid }}</div>
				</div>

				<div>
					<button
						@click.prevent="create()"
						class="group relative w-full flex justify-center py-2 px-4 border border-transparent text-sm font-medium rounded-md text-white bg-indigo-600 hover:bg-indigo-700 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-indigo-500"
					>
						<span
							class="absolute left-0 inset-y-0 flex items-center pl-3"
						>
							<!-- Heroicon name: solid/lock-closed -->
							<svg
								class="h-5 w-5 text-indigo-500 group-hover:text-indigo-400"
								xmlns="http://www.w3.org/2000/svg"
								viewBox="0 0 20 20"
								fill="currentColor"
								aria-hidden="true"
							>
								<path
									fill-rule="evenodd"
									d="M5 9V7a5 5 0 0110 0v2a2 2 0 012 2v5a2 2 0 01-2 2H5a2 2 0 01-2-2v-5a2 2 0 012-2zm8-2v2H7V7a3 3 0 016 0z"
									clip-rule="evenodd"
								/>
							</svg>
						</span>
						Add User
					</button>
					<div class="flex">
						<button
							@click.prevent="index(false)"
							class="group relative w-full flex justify-center py-2 px-4 border border-transparent text-sm font-medium rounded-md text-white bg-indigo-600 hover:bg-indigo-700 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-indigo-500"
						>
							<span
								class="absolute left-0 inset-y-0 flex items-center pl-3"
							>
								<!-- Heroicon name: solid/lock-closed -->
								<svg
									class="h-5 w-5 text-indigo-500 group-hover:text-indigo-400"
									xmlns="http://www.w3.org/2000/svg"
									viewBox="0 0 20 20"
									fill="currentColor"
									aria-hidden="true"
								>
									<path
										fill-rule="evenodd"
										d="M5 9V7a5 5 0 0110 0v2a2 2 0 012 2v5a2 2 0 01-2 2H5a2 2 0 01-2-2v-5a2 2 0 012-2zm8-2v2H7V7a3 3 0 016 0z"
										clip-rule="evenodd"
									/>
								</svg>
							</span>
							active
						</button>
						<button
							@click.prevent="index(true)"
							class="group relative w-full flex justify-center py-2 px-4 border border-transparent text-sm font-medium rounded-md text-white bg-indigo-600 hover:bg-indigo-700 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-indigo-500"
						>
							<span
								class="absolute left-0 inset-y-0 flex items-center pl-3"
							>
								<!-- Heroicon name: solid/lock-closed -->
								<svg
									class="h-5 w-5 text-indigo-500 group-hover:text-indigo-400"
									xmlns="http://www.w3.org/2000/svg"
									viewBox="0 0 20 20"
									fill="currentColor"
									aria-hidden="true"
								>
									<path
										fill-rule="evenodd"
										d="M5 9V7a5 5 0 0110 0v2a2 2 0 012 2v5a2 2 0 01-2 2H5a2 2 0 01-2-2v-5a2 2 0 012-2zm8-2v2H7V7a3 3 0 016 0z"
										clip-rule="evenodd"
									/>
								</svg>
							</span>
							Archive
						</button>
					</div>
				</div>
			</div>
		</div>
		<div>
			<!-- This example requires Tailwind CSS v2.0+ -->
			<div class="flex flex-col">
				<div class="-my-2 overflow-x-auto sm:-mx-6 lg:-mx-8">
					<div
						class="py-2 align-middle inline-block min-w-full sm:px-6 lg:px-8"
					>
						<div
							class="shadow overflow-hidden border-b border-gray-200 sm:rounded-lg"
						>
							<table class="min-w-full divide-y divide-gray-200">
								<thead class="bg-gray-50">
									<tr>
										<th
											scope="col"
											class="px-6 py-3 text-left text-xs font-medium text-gray-500 uppercase tracking-wider"
										>
											Name
										</th>

										<th
											scope="col"
											class="px-6 py-3 text-left text-xs font-medium text-gray-500 uppercase tracking-wider"
										>
											Email
										</th>
										<th
											scope="col"
											class="px-6 py-3 text-left text-xs font-medium text-gray-500 uppercase tracking-wider"
										>
											Archived
										</th>
										<th
											scope="col"
											class="relative px-6 py-3"
										>
											<span class="sr-only">Update</span>
										</th>
										<th
											scope="col"
											class="relative px-6 py-3"
										>
											<span class="sr-only">Delete</span>
										</th>
									</tr>
								</thead>
								<tbody
									class="bg-white divide-y divide-gray-200"
								>
									<tr v-for="u in users" :key="u.uuid">
										<td
											class="px-6 py-4 whitespace-nowrap text-sm font-medium text-gray-900"
										>
											<input
												type="text"
												v-model="u.name"
												name=""
											/>
										</td>
										<td
											class="px-6 py-4 whitespace-nowrap text-sm text-gray-500"
										>
											<input
												type="email"
												v-model="u.email"
												name=""
											/>
										</td>
										<td
											class="px-6 py-4 whitespace-nowrap text-sm text-gray-500"
										>
											<span v-if="u.is_archived"
												>Archived</span
											>
										</td>
										<td
											class="px-6 py-4 whitespace-nowrap text-right text-sm font-medium"
										>
											<button
												@click.prevent="update(u)"
												class="text-indigo-600 hover:text-indigo-900"
											>
												Update
											</button>
										</td>
										<td
											class="px-6 py-4 whitespace-nowrap text-right text-sm font-medium"
										>
											<button
												@click.prevent="del(u)"
												class="text-red-600 hover:text-indigo-900"
											>
												Delete
											</button>
										</td>
									</tr>
								</tbody>
							</table>
						</div>
					</div>
				</div>
			</div>
		</div>
	</div>
</template>

<script>
	export default {
		name: "HelloWorld",
		data() {
			return {
				user: {
					uuid: "",
					name: "Jason",
					is_archived: true,
					email: "derp@gmail.com",
					password: "password123",
				},
				db: null,
				users: [],
			};
		},
		computed: {},
		methods: {
			create() {
				window.console.log("Create triggered");
				this.user.uuid = Math.random(1000);
				var transaction = this.db.transaction(["users"], "readwrite");
				var users = transaction.objectStore("users");

				users.add(this.user);
				this.users.push(this.user);

				transaction.oncomplete = () => {
					console.log("User Created!");
				};
				transaction.onerror = (event) => {
					console.log(event.target.error);
				};
			},
			index(is_archived) {
				this.users = [];
				window.console.log("Index triggered");
				var users = this.db.transaction("users").objectStore("users");
				users.openCursor().onsuccess = (event) => {
					var cursor = event.target.result;
					if (cursor) {
						if (cursor.value.is_archived == is_archived) {
							this.users.push(cursor.value);
						}

						cursor.continue();
					} else {
						console.log("No more entries!");
					}
				};
			},
			update(object) {
				console.log(object.uuid);
				var objectStore = this.db
					.transaction(["users"], "readwrite")
					.objectStore("users");
				var request = objectStore.get(object.uuid);
				request.onerror = (event) => {
					console.log(event);
					console.log(
						"error while retrieving object to be updated from db."
					);
				};

				request.onsuccess = (event) => {
					var user = event.target.result;
					user = object;
					var requestUpdate = objectStore.put(user);
					requestUpdate.onerror = (event) => {
						console.log(event);
						console.log("error saving updated object");
					};
					requestUpdate.onsuccess = () => {
						console.log("successfully saved");
					};
				};
			},
			del(object) {
				console.log(object.uuid);
				var request = this.db
					.transaction(["users"], "readwrite")
					.objectStore("users")
					.delete(object.uuid);
				request.onsuccess = () => {
					console.log(object.uuid + " was deleted.");
					this.index();
				};
			},
			initializeDB() {
				var request = window.indexedDB.open("NewDB", 3);
				request.onupgradeneeded = (event) => {
					window.console.log("upgrade needed is called");
					this.db = event.target.result;
					this.db.createObjectStore("users", { keyPath: "uuid" });
					this.db.createObjectStore("deals", { keyPath: "uuid" });
					this.db.createObjectStore("lenders", { keyPath: "uuid" });
				};
				request.onsuccess = (event) => {
					this.db = event.target.result;
					window.console.log(event);
					window.console.log("InitializeDB Success.");
				};
				request.onerror = (event) => {
					console.error("Database error: " + event.target.errorCode);
				};
			},
		},
		mounted() {
			this.initializeDB();
		},
	};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped></style>
