<template>
	<div class="p-8 flex w-full">
		<!-- Left Column -->
		<div class="w-3/4 pr-4">
			<!-- Header -->
			<div class="pt-4">
				<h1 class="text-3xl font-bold ">
					{{ name }}
				</h1>
				<h2 class="text-xl font-bold text-orange-600">
					{{ profession }}
				</h2>
				<div>
					{{ location }}
				</div>
			</div>
			<!-- Profile -->
			<div class="pt-4">
				<h2 class="text-lg font-bold text-orange-600">
					Profile
				</h2>
				<div class="border-l-4 pl-5 text-sm">
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
			<div class="pt-4">
				<h2 class="text-lg font-bold text-orange-600">
					Experience
				</h2>
				<div class="border-l-4 pl-4">
					<div
						v-for="(item, index) in experience"
						:key="index"
						class="py-2"
					>
						<h3 class="text-md font-semibold text">
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
								<p class="text-sm text-gray-600">
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
			<div class="border-l-4 pl-4">
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
			</div>
		</div>
	</div>
</template>

<script>
	export default {
		data() {
			return {
				test: "data",
				name: "Jason Law",
				profession: "Real Estate Sales Agent",
				location: "North Lakes, Queensland, Australia",
				profile: [
					"Sales experience - 16 years in various roles and industries",
					"Able to perform under considerable time and target pressures",
					"Fun, friendly and generous personality with a contagious enthusiasm",
					"Very strong record-keeping habits for client notes within CRM",
					"High integrity sales ethos, focussed on ownership",
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
						title: "Systems",
						content: [
							"Zoho CRM",
							"Hubspot CRM",
							"Asana",
							"Office 365",
							"Salesforce CRM",
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
									"Finance Property Wealth Group is a combination of mortgage brokerage and investment property sales, my role is onboarding clients and managing their progress through our business.",
									"I visit clients in their home to introduce our business and set expectations. Client appointments are set by our telemarketing team and indicate that the prospect has an interest in refinancing their mortgage or buying some Investment Property.",
									"",
								],
							},
							{
								position: "Real Estate Sales Agent",
								employer: "Webster's Property Partners",
								from: "July 2020",
								to: "February 2021",
								tenure: "7m",
								description: [
									"I was employed in the start-up Property Sales division of Webster's Wealth Partners, initially established to sell house and land packages to First Home Buyers, this focus later changed to target investors.",
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
								employer: "Hobby & small projects",
								from: "January 2018",
								to: "Present",
								tenure: "4y",
								description: [
									"I've built various small projects for work and enjoyment. This resume is built as a web application, for example.",
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
									"Beginning July 2019, when Auto Approve was acquired by Auto Sports Group Limited, I transitioned to full-time Account Manager for the brokerage, maintaining its referral partner dealerships in Brisbane.",
									"I Maintained relationships and contact with referral partner business managers on a regular basis and took credit applications from their clients. Also made myself available as a Locum Business Manager for the group of Dealerships over the Christmas and New Year season to demonstrate our company's commitment to their success.",
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
									"This employer was a training academy, intended to give training and experience to cadetBusiness Managers by placing them into dealerships as cheap locums.",
									"The role was intended to be temporary and last no longer than 18 months before thecadet became ready to enter the market on their own.",
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
									"Customer support role. Contact centre based in Ann Street assisting Telstra BusinessClients with 􀁽xed line and mobile faults and provisioning.",
								],
							},
							{
								position: "Inbound Sales",
								employer: "3 Mobile",
								from: "May 2008",
								to: "June 2010",
								tenure: "2y1m",
								description: [
									"Inbound sales calls assisting people who would respond to direct mail, TV and radioadvertising. Goal was to close on the 􀁽rst call and provision the service over the phone.",
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
									"Sales of pumps and accessories. This role was primarily phone based to assist customerswho called to get expert knowledge on Pump selection.",
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
									"Junior retail traineeship. Sales of pumps and electric motors, power tools and equipment.",
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
