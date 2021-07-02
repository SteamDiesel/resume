<template>
  <div>
      {{experience}}
  </div>
</template>

<script>
export default {
    data(){
        return {
            test: "data",
            profile: [
                "Sales experience - 18 years in various roles and industries",
                "Able to perform under considerable time and target pressures",
                "Fun, friendly and generous personality with a contagious enthusiasm",
                "Very strong record-keeping habits for client notes within CRM",
                "High integrity sales ethos, focussed on ownership",
                "Clear and effective communicator by all mediums with an excellent phonemanner",
                "PC Power-User with hobby projects as a full stack web developer"
            ],
            experience: [
                {
                    career: "Real Estate Sales",
                    length: "1 year",
                    roles: [
                        {
                            position: "Real Estate Sales Agent",
                            employer: "Webster's Property Partners",
                            from: "July 2020",
                            to: "February 2021",
                            tenure: "7m",
                            description: [
                                "I was employed in the start-up Property Sales division of Webster's Wealth Partners,initially established to sell house and land packages to First Home Buyers, this focus laterchanged to target investors.",
                                "I established the Zoho CRM into the business where there was previously no CRM orformal sales process.",
                                "I created entire sales scripts, tools and automation to streamline and improve the efficiency of lead outreach.",
                                "I researched land and put together several deals with clients for House and Land packages.",
                                "I also made signi􀁽cant contributions to help with dev-ops for the website and other digital infrastructure for the business.",
                                "Where there was no process for selling, I created one as I went. I had expected that myefforts here would be useful to future staff as our team would eventually grow.",
                            ]
                        }
                    ]
                }
            ]
        }
    }
}
</script>

<style>

</style>