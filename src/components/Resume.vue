<template>
	<div class="p-12 print:p-2 flex w-full tracking-wide">
		<!-- Left Column -->
		<div class="w-3/4 pr-4">
			<!-- Header -->
			<div class="pt-4 flex">
				<div class="w-28">
					<svg viewBox="-13 0 511 512">
						<path
							d="m328.554688 480.546875c0 17.371094-14.082032 31.453125-31.453126 31.453125-17.371093 0-31.453124-14.082031-31.453124-31.453125s14.082031-31.453125 31.453124-31.453125c17.371094 0 31.453126 14.082031 31.453126 31.453125zm0 0"
							fill="#f6ad55"
						/>
						<path
							d="m328.554688 480.546875c0 17.371094-14.082032 31.453125-31.453126 31.453125 0-31.453125 0-39.601562 0-62.90625 17.371094 0 31.453126 14.082031 31.453126 31.453125zm0 0"
							fill="#dd6b20"
						/>
						<path
							d="m63.40625 399.25c0 17.371094-14.082031 31.453125-31.453125 31.453125s-31.453125-14.082031-31.453125-31.453125 14.082031-31.453125 31.453125-31.453125 31.453125 14.082031 31.453125 31.453125zm0 0"
							fill="#f6ad55"
						/>
						<path
							d="m63.40625 399.25c0 17.371094-14.082031 31.453125-31.453125 31.453125 0-31.453125 0-46.808594 0-62.90625 17.371094 0 31.453125 14.082031 31.453125 31.453125zm0 0"
							fill="#dd6b20"
						/>
						<path
							d="m485.210938 375.335938c0 17.367187-14.082032 31.449218-31.453126 31.449218-17.371093 0-31.453124-14.082031-31.453124-31.449218 0-17.371094 14.082031-31.453126 31.453124-31.453126 17.371094 0 31.453126 14.082032 31.453126 31.453126zm0 0"
							fill="#f6ad55"
						/>
						<path
							d="m485.210938 375.335938c0 17.367187-14.082032 31.449218-31.453126 31.449218 0-31.449218 0-38.988281 0-62.902344 17.371094 0 31.453126 14.082032 31.453126 31.453126zm0 0"
							fill="#dd6b20"
						/>
						<path
							d="m432.203125 85.230469c0-24.320313-19.714844-44.035157-44.035156-44.035157-16.214844 0-30.375 8.773438-38.015625 21.824219-12.617188-5.425781-26.515625-8.4375-41.121094-8.4375-13.710938 0-26.804688 2.65625-38.792969 7.46875-16.183593-36.546875-52.761719-62.050781-95.304687-62.050781-57.539063 0-104.183594 46.644531-104.183594 104.183594 0 25.871094 9.4375 49.539062 25.050781 67.757812-15.613281 18.214844-25.050781 41.882813-25.050781 67.757813 0 45.878906 29.65625 84.832031 70.847656 98.734375v131.910156c0 15.476562 12.546875 28.023438 28.023438 28.023438 15.480468 0 28.027344-12.546876 28.027344-28.023438v-128.957031c40.730468-9.0625 72.488281-41.957031 79.847656-83.300781 9.949218 3.152343 20.542968 4.863281 31.535156 4.863281 2.746094 0 5.46875-.109375 8.164062-.316407v91.722657c0 15.476562 12.546876 28.023437 28.023438 28.023437 15.480469 0 28.027344-12.546875 28.027344-28.023437v-113.546875c24.332031-19.070313 39.96875-48.730469 39.96875-82.042969 0-11.902344-2-23.332031-5.675782-33.988281 14.605469-7.167969 24.664063-22.179688 24.664063-39.546875zm0 0"
							fill="#f6ad55"
						/>
						<path
							d="m432.203125 85.230469c0-24.320313-19.714844-44.035157-44.035156-44.035157-16.214844 0-30.375 8.773438-38.015625 21.824219-12.617188-5.425781-26.515625-8.4375-41.121094-8.4375-13.710938 0-26.804688 2.65625-38.792969 7.46875-6.308593-14.246093-15.730469-26.804687-27.382812-36.839843v293.457031c17.785156-15.308594 30.355469-36.507813 34.640625-60.582031 9.949218 3.152343 20.542968 4.863281 31.535156 4.863281 2.746094 0 5.46875-.109375 8.164062-.316407v91.722657c0 15.476562 12.546876 28.023437 28.023438 28.023437 15.480469 0 28.027344-12.546875 28.027344-28.023437v-113.546875c24.332031-19.070313 39.96875-48.730469 39.96875-82.042969 0-11.902344-2-23.332031-5.675782-33.988281 14.605469-7.167969 24.664063-22.179688 24.664063-39.546875zm0 0"
							fill="#dd6b20"
						/>
					</svg>
				</div>
				<div class="pl-4">
					<h1 class="text-3xl font-bold text-gray-600 mt-3">
						{{ name }}
					</h1>
					<h2 class="text-xl font-bold text-orange-600">
						{{ profession }}
					</h2>
					<div class="flex text-gray-500 text-sm mt-1">
						<svg class="h-4 pr-2" viewBox="0 0 384 512">
							<path
								fill="currentColor"
								d="M172.268 501.67C26.97 291.031 0 269.413 0 192 0 85.961 85.961 0 192 0s192 85.961 192 192c0 77.413-26.97 99.031-172.268 309.67-9.535 13.774-29.93 13.773-39.464 0zM192 272c44.183 0 80-35.817 80-80s-35.817-80-80-80-80 35.817-80 80 35.817 80 80 80z"
							></path>
						</svg>
						{{ location }}
					</div>
				</div>
			</div>
			<!-- Profile -->
			<div class="pt-10">
				<h2 class="text-lg font-bold text-orange-600">
					Profile
				</h2>
				<div class="border-l-2 pl-5 text-sm">
					<div
						v-for="(line, index) in profile"
						:key="index"
						class="my-1"
					>
						{{ line }}
					</div>
				</div>
			</div>
			<!-- Experience -->
			<div class="pt-10">
				<h2 class="text-lg font-bold text-orange-600">
					Experience
				</h2>
				<div class="border-l-2 pl-4">
					<div
						v-for="(item, index) in experience"
						:key="index"
						class="py-2"
					>
						<h3 class="text-md font-semibold text-gray-600">
							{{ item.career }} [{{ item.tenure }}]
						</h3>
						<div class="border-l-2 pl-4">
							<div
								v-for="(role, index) in item.roles"
								:key="index"
								class="mb-3"
							>
								<h4
									class="text-md font-semibold text-orange-600"
								>
									{{ role.position }}
								</h4>
								<p
									class="text-sm font-semibold text-gray-600 mb-1"
								>
									{{ role.employer }} | {{ role.from }} -
									{{ role.to }} [{{ role.tenure }}]
								</p>
								<p
									v-for="(line, index) in role.description"
									:key="index"
									class="text-xs"
								>
									{{ line }}
								</p>
							</div>
						</div>
					</div>
				</div>
			</div>
		</div>
		<!-- Right Column -->
		<div class="w-1/4">
			<div class="border-l-2 pl-4">
				<div class="mb-10">
					<h2 class="text-md font-semibold text-orange-600 mb-2">
						Details
					</h2>
					<div
						v-for="(item, index) in details"
						:key="index"
						class="text-sm mb-2"
					>
						{{ item.line }}
					</div>
				</div>
				<div v-for="(item, index) in lists" :key="index" class="mb-10">
					<h2 class="text-md font-semibold text-orange-600 mb-2">
						{{ item.title }}
					</h2>
					<div
						v-for="(line, index) in item.content"
						:key="index"
						class="text-sm mb-2"
					>
						{{ line }}
					</div>
				</div>
				<div class=" w-24">
					<div class="flex mx-auto my-auto">
						<svg class="h-16 text-orange-100" viewBox="0 0 640 512">
							<path
								fill="currentColor"
								d="M278.9 511.5l-61-17.7c-6.4-1.8-10-8.5-8.2-14.9L346.2 8.7c1.8-6.4 8.5-10 14.9-8.2l61 17.7c6.4 1.8 10 8.5 8.2 14.9L293.8 503.3c-1.9 6.4-8.5 10.1-14.9 8.2zm-114-112.2l43.5-46.4c4.6-4.9 4.3-12.7-.8-17.2L117 256l90.6-79.7c5.1-4.5 5.5-12.3.8-17.2l-43.5-46.4c-4.5-4.8-12.1-5.1-17-.5L3.8 247.2c-5.1 4.7-5.1 12.8 0 17.5l144.1 135.1c4.9 4.6 12.5 4.4 17-.5zm327.2.6l144.1-135.1c5.1-4.7 5.1-12.8 0-17.5L492.1 112.1c-4.8-4.5-12.4-4.3-17 .5L431.6 159c-4.6 4.9-4.3 12.7.8 17.2L523 256l-90.6 79.7c-5.1 4.5-5.5 12.3-.8 17.2l43.5 46.4c4.5 4.9 12.1 5.1 17 .6z"
							></path>
						</svg>
					</div>
				</div>
			</div>
		</div>
	</div>
</template>

<script>
	export default {
		data() {
			return {
				name: "Jason Law",
				profession: "Real Estate Sales Agent",
				location: "North Lakes, Queensland, Australia",
				profile: [
					"Sales experience - 16 years in various roles and industries",
					"Keen interest in developing further negotiation skills",
					"High integrity sales ethos assuming ownership of client outcomes",
					"Able to perform under considerable time and target pressure",
					"Fun, friendly and enthusiastic with a team building attitude",
					"Very strong record-keeping habits for client notes within CRM",
					"Clear and effective communicator by all mediums with an excellent phone manner",
					"Bonus skills as a full-stack web developer",
				],
				details: [
					{
						line: "Australian Citizen, M, 35",
						url: "",
					},
					{
						line: "0400 696 332",
						url: "tel:0400696332",
					},
					{
						line: "jason.lloyd.law@gmail.com",
						url: "mailto:jason.lloyd.law@gmail.com",
					},
					{
						line: "github.com/SteamDiesel",
						url: "https//github.com/SteamDiesel",
					},
					{
						line: "linkedin.com/in/jason-lloyd-law",
						url: "https//linkedin.com/in/jason-lloyd-law",
					},
				],
				lists: [
					{
						title: "Valued Skills",
						content: [
							"Sales",
							"Negotiation",
							"Prospecting",
							"Lead Management",
							"Client Management",
							"Web Development",
						],
					},
					{
						title: "Systems",
						content: [
							"Zoho CRM",
							"Hubspot CRM",
							"Salesforce CRM",
							"Asana",
							"Office 365",
							"G-Suite",
						],
					},
					{
						title: "Certifications",
						content: [
							"Cert IV Finance & Mortgage Broking",
							"Cert IV in Property Services (Real Estate)",
							"RG146 Tier 2 - General Advice (General Insurance)",
						],
					},
					{
						title: "Web Stack",
						content: [
							"Laravel",
							"PHP",
							"VueJS",
							"Javascript",
							"Tailwind CSS",
							"MySQL",
						],
					},
				],
				experience: [
					{
						career: "Real Estate Sales",
						tenure: "1 year",
						roles: [
							{
								position: "Investment Property Consultant",
								employer: "FPW Group",
								from: "February 2021",
								to: "Present",
								tenure: "4m",
								description: [
									"Finance Property Wealth Group consists primarily of a mortgage brokerage and investment property sales team, my role is onboarding clients and managing their progress through our business.",
									"Client appointments are set by our telemarketing team and indicate that the prospect has an interest in refinancing their mortgage or buying some Investment Property.",
									"I visit clients in their home to introduce our business and set expectations. ",
								],
							},
							{
								position: "Real Estate Sales Agent",
								employer: "Webster's Property Partners",
								from: "July 2020",
								to: "February 2021",
								tenure: "7m",
								description: [
									"I was employed in the start-up Property Sales division of Webster's Wealth Partners, initially established to sell house and land packages to First Home Buyers, the focus of this project later changed to target investors.",
									"I established the Zoho CRM into the business where there was previously no CRM or formal sales process.",
									"I created entire sales scripts, tools and automation to streamline and improve the efficiency of lead outreach.",
									"I researched land and put together several deals with clients for House and Land packages.",
									"I also made significant contributions to help with development and operations of the website and other digital infrastructure for the business.",
									"Where there was no process for selling, I created one as I went. I had expected that my efforts here would be useful to future staff as our team would eventually grow.",
								],
							},
						],
					},
					{
						career: "Full Stack Web Developer",
						tenure: "3 years",
						roles: [
							{
								position: "Full Stack Web Developer",
								employer: "Various projects",
								from: "January 2018",
								to: "Present",
								tenure: "3y",
								description: [
									"I've built various projects for work and enjoyment. This resume is built as a web application, for example.",
									"I am most proud of the Finance Brokerage CRM that I built as a VueJS single page application with a Laravel API for access control, database queries and business logic.",
									"I have found it quick and easy to spin up small javascript projects to make custom tools and toolboxes for work that are extremely powerful and flexible.",
								],
							},
						],
					},
					{
						career: "Sales & Finance - Motor Trade",
						tenure: "8 years",
						roles: [
							{
								position: "Sales & Finance - Business Manager",
								employer: "AutoApprove",
								from: "September 2018",
								to: "March 2020",
								tenure: "1y7m",
								description: [
									"Beginning July 2019, when Auto Approve was acquired by Auto Sports Group Limited, I transitioned to full-time Account Manager for the brokerage, maintaining its referral-partner dealerships in Brisbane.",
									"I Maintained relationships and contact with referral-partner business managers on a regular basis and took credit applications from their clients. Also made myself available as a Locum Business Manager for the group of Dealerships over the Christmas and New Year season to demonstrate our company's commitment to their success.",
								],
							},
							{
								position:
									"Sales & Finance - Locum Business Manager",
								employer: "Sole Trader",
								from: "September 2013",
								to: "January 2019",
								tenure: "4y5m",
								description: [
									"As a locum BM, I kept my calendar booked up by ensuring I maintained regular contact with all of my contacts within the motor trade in the greater Brisbane region.",
									"Within the dealerships, my role is to Sell the dealership's finance and insurance options. While at a higher level my role as a sole trader was to ensure I was keeping my calendar consistently booked.",
									"During my time as a Locum BM, I have worked in nearly 100 different car dealerships on the east coast of Australia.",
								],
							},
							{
								position: "Sales & Finance - Finance Broker",
								employer: "Sole Trader",
								from: "September 2014",
								to: "January 2019",
								tenure: "3y5m",
								description: [
									"As a Finance Broker, I assisted my clients to secure approvals for loans on vehicles and equipment.",
									"As a sole trader, I relied on both lead generation and prospecting as well as building and strengthening my referral relationships.",
								],
							},
							{
								position:
									"Sales & Finance - Cadet Locum Business Manager",
								employer: "MTA Insurance",
								from: "January 2012",
								to: "January 2013",
								tenure: "1y",
								description: [
									"This employer was a training academy, intended to give training and experience to cadet Business Managers by placing them into dealerships as cheap locums.",
									"The role was intended to be temporary and last no longer than 18 months before the cadet became ready to enter the market on their own.",
								],
							},
						],
					},
					{
						career: "Sales & Service - Telco",
						tenure: "3 years",
						roles: [
							{
								position: "Business Customer Support",
								employer: "Telstra",
								from: "July 2010",
								to: "July 2011",
								tenure: "1y",
								description: [
									"Customer support role. Contact centre based in Ann Street assisting Telstra Business Clients with fixed line and mobile faults and provisioning.",
								],
							},
							{
								position: "Inbound Sales",
								employer: "3 Mobile",
								from: "May 2008",
								to: "June 2010",
								tenure: "2y1m",
								description: [
									"Inbound sales calls assisting people who would respond to direct mail, TV and radio advertising. Goal was to close on the first call and provision the service over the phone.",
								],
							},
						],
					},
					{
						career: "Sales - Pumping and Irrigation",
						tenure: "4 years",
						roles: [
							{
								position: "Advanced Technical Sales",
								employer: "McCracken's Water Services",
								from: "March 2006",
								to: "May 2008",
								tenure: "2y2m",
								description: [
									"Sales of pumps and accessories. This role was primarily phone based to assist customers who called to get expert knowledge on Pump selection.",
									"Success in this role was dependent on the level of product knowledge and conveying confidence in selection to the customer.",
								],
							},
							{
								position: "Technical Sales",
								employer: "The Electrical Workshop",
								from: "March 2003",
								to: "August 2004",
								tenure: "2y1m",
								description: [
									"Junior retail trainee. Sales of pumps and electric motors, power tools and equipment.",
								],
							},
						],
					},
				],
			};
		},
	};
</script>

<style></style>
