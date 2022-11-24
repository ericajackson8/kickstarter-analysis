
# Kickstarting with Excel

## Overview of Project
This project is an analysis of data from various crowdfunding campaigns across various categories and subcategories. The data reflects the name and and a short description of the campaign with other campaign level performance and outcomes.

### Purpose
The purpose of this project is to assist an up-and-coming playwright, Lousie, plan a crowdfunding campaign for her new play, Fever. The hope is that we could identify success factors from previous theater campaigns and provide these insights to Louise to increase the probability of a successful campaign launch for her play, Fever.
## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
To gain some insight about the outcomes based on when the theater program was launched, a pivot table was used to show the distribution of outsomes by the month the campaign was launched. To give a more visual view a line graph was created to show the trend.
Across all categories in general, and theater in particular, it appears that the number of successful campaigns spikes in May and gradually decreases to a low in September before rebounding.  In December, the number of successful and failed campaigns are virtually equal. The campaign outcome could very well be seasonal; in the Spring/Summer, successful campaigns increase because the weather and then vacation season; whereas, in December Holiday activities are prioritized over non-holiday activities. 
[Theater_Outcomes_vs_Launch.png](https://github.com/ericajackson8/kickstarter-analysis/blob/main/Resources/Theater_Outcomes_vs_Launch.png))

### Analysis of Outcomes Based on Goals
To gain insight on campaign outcomes based on the goal amount we created a chart to calculate the percentage of each outcome by discrete ranges of goal amount.  We utilize the COUNTIFS to summarize the number of campaigns within each outcome and goal amount range. From here, we created another line chart to provide a visual of the outcome percentages by goal amount.
Campaigns less than $5,000 are the most successful with a success rate of 73%. The percentage of successful campaigns decreases at goal amounts above $5,000.  Goal amounts between $35,000 and $45,000 apear to be almost as successful as small campaigs, however, the overall volume of campaigns is low here so results are less reliable here. 
### Challenges and Difficulties Encountered
Challenges were few.  After creating the second analysis, I noticed that my resulting chart was different. I began taking a look at what I needed to modify to get teh intended results.  Through this process, I was able to continue to explore and familiarize myself with additional charting options and features.  I even used google to identify some additional resources.  Ultimately, I went back to the requirements and realized that I had forgotten the subcategory filter on plays. I needed to go back to my Outcomes Based on Goals chart and add an additional condition to my COUNTIFS statement. Once I did this, everything was good.
## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
  1. The outcome of the campaign is seasonal and so launching a campaign in the Spring/Summer (May - July) has higher probability of a successful outcome.
  2. Avoid launching campaigns in December where the volume of successful and failed campaigns are virtually equal.

- What can you conclude about the Outcomes based on Goals?
    Smaller goal amounts are more likely to be successful so, I recommend lowering the goal amount and having multiple campaigns.
- What are some limitations of this dataset?
    More campaign specific data like the platform.  Knowing the platform and some additional specifics about the operational aspects of the campaign would definitely help to understand the outcomes.
    More detail and context around the fields, in particular, understanding of the staff_pick and spotlight data.
    Understanding of how Successful vs. Failed was defined.  For example, is Successful based on the ration of Pledged to Goal being greater than a certain threshold.  If so, understanding this detail would be good, because there might be alternative ways to conclude Success.

- What are some other possible tables and/or graphs that we could create?

    We could have looked at the %Percentage of each Outcome by Month, instead of just looking at the volume.
