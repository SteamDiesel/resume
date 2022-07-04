<template>
	<div class="p-14 print:p-2 flex w-full tracking-wide">
		<!-- Left Column -->
		<div class="w-full sm:w-3/4 pr-4">
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
						{{ position }}
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
				<h2 class="text-lg font-bold text-orange-600">Profile</h2>
				<div class="border-l-2 pl-8 text-sm">
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
			<div class="pt-10 pr-4">
				<h2 class="text-lg font-bold text-orange-600">Experience</h2>
				<div class="border-l-2 pl-8">
					<div
						v-for="(item, index) in experience"
						:key="index"
						class="pt-4 mb-8"
					>
						<h3 class="text-md font-semibold text-gray-600">
							{{ item.career }} [{{ item.tenure }}]
						</h3>
						<div class="border-l-2 pl-8">
							<div
								v-for="(role, index) in item.roles"
								:key="index"
								class="pt-2 no-break"
							>
								<h4
									class="
										text-md
										font-semibold
										text-orange-600
									"
								>
									{{ role.position }}
								</h4>
								<p
									class="
										text-sm
										font-semibold
										text-gray-600
										mb-1
									"
								>
									{{ role.employer }} | {{ role.from }} -
									{{ role.to }} [{{ role.tenure }}]
								</p>
								<p
									v-for="(line, index) in role.description"
									:key="index"
									class="text-xs mb-1"
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
		<div class="w-1/4 hidden sm:block">
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
						<a
							v-if="item.url"
							target="blank"
							:href="item.type + item.url"
							>{{ item.line }}</a
						>

						<span v-if="!item.url">{{ item.line }}</span>
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
				<div class="w-24">
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
	props: {
		name: String,
		position: String,
	},
	data() {
		return {
			location: "North Lakes, Queensland, Australia",
			profile: [
				"Sales experience - 17 years in various roles and industries",
				"Seeking opportunities to develop advanced negotiation skills",
				"High integrity sales ethos assuming ownership of client outcomes",
				"Able to perform under considerable time and target pressure",
				"Fun, friendly and enthusiastic with a team building attitude",
				"Very strong record-keeping habits for client notes within CRM",
				"Clear and effective communicator by all mediums with an excellent phone manner",
				"Open QLD drivers licence with a clean driving record",
				"Bonus skills as a full-stack web developer",
			],
			details: [
				{
					line: "Australian Citizen, M, 36",
					url: "",
					type: "",
				},
				{
					line: "",
					url: "",
					type: "",
				},
				{
					line: "0400 696 332",
					url: "0400696332",
					type: "tel:",
				},
				{
					line: "jason.lloyd.law@gmail.com",
					url: "jason.lloyd.law@gmail.com",
					type: "mailto:",
				},
				{
					line: "github.com/SteamDiesel",
					url: "github.com/SteamDiesel",
					type: "https://",
				},
				{
					line: "linkedin.com/in/jason-lloyd-law",
					url: "linkedin.com/in/jason-lloyd-law",
					type: "https://",
				},
			],
			lists: [
				{
					title: "Valued Skills",
					content: [
						"Negotiation",
						"Lead Management",
						"Web Development",
						"Product Management",
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
						"inertiajs",
						"Javascript",
						"Tailwind CSS",
						"MySQL",
					],
				},
			],
			experience: [
				{
					career: "Full Stack Web Developer",
					tenure: "4 years",
					roles: [
						{
							position: "Technical Founder / Product Manager",
							employer: "Garaji.me",
							from: "March 2022",
							to: "Present",
							tenure: "4m",
							description: [
								"Garaji.me is a complex and ambitious project to catalogue all vehicle information and provide users with a place to manage their cars history and maintenance.",
								"I am the sole web developer on this project, responsible for all decisions. I am responsible for UI and UX, design and layout and technical implementation decisions.",
								"Laravel with inertiajs, using laravel nova as the dashboard. Tailwind CSS and using the Tailwind UI component library.",
							],
						},
						{
							position: "Product Manager",
							employer: "OurProperty",
							from: "January 2022",
							to: "Present",
							tenure: "6m",
							description: [
								"Responsible for implementing the front-end support dashboard for administrative investigation and changes. I am responsible for the API spec and ensuring the quality of those API endpoints from the offshore development team.",
								"Working in the support team to understand the need for tools to improve support response times and capabilities.",
								"Working on this project as the sole developer, I am responsible for UI and UX, design and layout and implementation decisions.",
								"Laravel with inertiajs, using laravel nova as the dashboard. Tailwind CSS and using the Tailwind UI component library.",
							],
						},
						{
							position:
								"Business Development Manager & Web Developer",
							employer:
								"Broker & Dealer Finance & Insurance (BDFI)",
							from: "February 2020",
							to: "Present",
							tenure: "2y4m",
							description: [
								"After my exposure to the challenges of working in motor trade finance, I created a custom CRM system for Dealership Business Managers and Finance Brokers.",
								"This CRM includes lead & application management, task management and point of sale tools that dramatically improve the speed and efficiency of operations within an asset finance pipeline.",
								"As the sole developer and sales rep for this early-stage SAAS start-up, I am responsible for both product development and customer acquisition. I've performed market research and testing with my fellow industry contacts to gather feedback and improve the product-market-fit.",
								"The BDFI application has been built in my spare time and is a 'minimum viable product' which is in the market for testing and feedback.",
								"The development of BDFI has been a passion project, which I've used to improve my own coding skills.",
							],
						},
						{
							position: "Freelance Web Developer",
							employer: "SteamDiesel.dev",
							from: "January 2018",
							to: "Present",
							tenure: "4y",
							description: [
								"I've built various projects for work and enjoyment. This resume is built as a web application, for example.",
								"I am most proud of the memorial site I built for kingkai.org, which I built as a VueJS single page application with a Laravel API for access control, database queries and business logic.",
								"I have found it quick and easy to spin up small javascript projects to make custom tools and toolboxes for work that are extremely powerful and flexible.",
							],
						},
					],
				},
				{
					career: "Sales Executive / Representative",
					tenure: "7y",
					roles: [
						{
							position: "Business Development Manager",
							employer: "National Property Group",
							from: "November 2021",
							to: "Present",
							tenure: "3m",
							description: [
								"Developing a detailed understanding of the NPD business, customers, relationships and products",
								"Proactively and constantly find and close opportunities, cold call prospects via telephone and personal selling and follow-up on prospective leads",
								"Source and maintain accurate contact information and distribution lists",
								"Maintain a thorough understanding of assigned territory and National Property Data Limited's market positioning",
								"Negotiate and close deals and manage sales pipeline",
								"Prepare and run onsite demonstrations",
								"Assist with area meetings and demonstrations",
								"Maintain an expert's understanding of all National Property Data Limited's products and services",
								"Perform daily maintenance and updates of the CRM system",
							],
						},
						{
							position: "Investment Property Consultant",
							employer: "FPW Group",
							from: "February 2021",
							to: "October 2021",
							tenure: "8m",
							description: [
								"Finance Property Wealth Group consists primarily of a mortgage brokerage and investment property sales, my role was onboarding clients and managing their expectations and progress through our business.",
								"My Role involved helping clients accomplish financial objectives by assessing their financial situation, developing and presenting financial strategies and plans, and monitoring changes in financial status and life circumstances. ",
								"My client appointments were set by our telemarketing team and indicate that the prospect has an interest in refinancing their mortgage or buying some Investment Property. This meant that the marketing agent was also interested in the outcome of the meeting with their prospect, so I kept them informed with progress and feedback.",
								"For the majority of appointments, I would visit clients in their home to introduce our business and set expectations.",
								"The goal of my initial meeting with clients was to clearly articulate the value of our business to prospective investors while getting to know the client's personal & financial situation.",
								"When a client proceeds to buy an investment property with us, it was my responsibility to maintain momentum and engagement with the client from finance, property selection, settlement and completion.",
							],
						},

						{
							position: "Property Sales Consultant",
							employer: "Webster's Property Partners",
							from: "July 2020",
							to: "February 2021",
							tenure: "7m",
							description: [
								"I was employed in the start-up Property Sales division of Webster's Wealth Partners, initially established to sell house and land packages, townhouses and units to First Home Buyers. Before shutting down, this division began to service investors.",
								"Webster's is a group of Financial planners, Accountants and Property Managers. These businesses are either related or in service to wealth creation and investment.",
								"I established the Zoho CRM into the business where there was previously no CRM or formal sales process.",
								"I created entire sales scripts, tools and automation to streamline and improve the efficiency of lead outreach.",
								"I researched land and put together several deals with clients for House and Land packages.",
								"I made significant contributions to the development and operations of the website and other digital infrastructure for the business.",
								"I scripted, shot and edited video advertisements which were used to promote the business and offerings. ",
								" ",
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
								"My time as a sole trader and finance closer within various dealerships has substantially improved my sales and business acumen.",
								"I positioned myself as 'the guy to call if you need a locum' by ensuring that I knew and collaborated with other locums. If a dealership called me and I was unable to work their booking, I would call my network and find a locum to do the job.",
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
								"A finance client is a buyer like any other, motivated by cost and convenience. My ability to make income depends heavily on my ability to built trust and rapport while also maintaining a high level of service and control over the sale.",
								"As a sole trader, I relied on my own lead generation and prospecting as well as building and strengthening referral relationships.",
							],
						},
						{
							position: "Business Development Manager",
							employer: "AEncompas",
							from: "July 2010",
							to: "July 2011",
							tenure: "12m",
							description: [
								"Start up telco business reselling Telstra, Optus, Vodafone and various other business phone plans for commission.",
								"Role involved typical sales rep duties of prospecting via cold calling and canvassing businesses in person.",
								"",
							],
						},
						{
							position: "Outbound B2B Lead Generation",
							employer: "3 Mobile - Call Centre",
							from: "February 2009",
							to: "October 2009",
							tenure: "8m",
							description: [
								"This role was in a new and experimental lead generation team started with me and some other high performing sales agents from various departments.",
								"The Lead-Gen team was responsible for calling cold business data and setting appointments for our Business Sales team to visit and convert accounts.",
								"This was my first outbound role, but I quickly adapted to the call volume and built personal resilience against the high rejection nature of outbound sales.",
								"This team was disbanded when the Vodafone takeover was announced and I returned to my previous Inbound Sales role.",
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
								"A business manager in a motor dealership sees every single client and tries to sell finance and insurance products.",
								"I had a deep and broad understanding of sales and finance by this stage and so I put them to good use. I helped to close more deals and inject more energy into this sleepy little dealership.",
								"Beginning July 2019, when Auto Approve was acquired by Auto Sports Group Limited, I transitioned to full-time Account Manager for the brokerage, maintaining its referral-partner dealerships in Brisbane.",
								"I Maintained relationships and contact with referral-partner business managers on a regular basis and took credit applications from their clients. Also made myself available as a Locum Business Manager for the group of Dealerships over the Christmas and New Year season to demonstrate our company's commitment to their success.",
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
								"At this time Telstra had a reputation for call centre transfer hell. Thankfully however, we had more freedom and time to fix client issues and give our clients a better experience in this department.",
								"We were responsible for ensuring that we solved the client's problem while on the client's call, with the ability to make outbound calls and follow up to ensure follow through on our promises to clients.",
							],
						},

						{
							position: "Inbound Sales",
							employer: "3 Mobile - Call Centre",
							from: "May 2008",
							to: "June 2010",
							tenure: "2y1m",
							description: [
								"Inbound sales calls assisting people who would respond to direct mail, TV and radio advertising. My goal was to close the sale on the first call and provision the service over the phone.",
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
								"Sales of household and agricultural pumps and plumbing accessories. This role was primarily phone-based to assist customers with expert knowledge on pump selection.",
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
								"I started my sales career as a Junior retail trainee. In this role, I sold water pumps, electric motors, power tools and equipment to consumer and trade customers.",
								"Sales of household and agricultural pumps and plumbing accessories. Success in this role was dependent on the level of product knowledge and a can-do attitude.",
							],
						},
					],
				},
			],
		};
	},
};
</script>

<style>
.no-break {
	page-break-inside: avoid;
}
</style>
