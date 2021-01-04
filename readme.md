# Which prepaid plan is more profitable?

### Background

This project is part of the Data Scientist training program from Practicum by Yandex. More info in link below:

https://practicum.yandex.com/data-scientist 

### Project Setup

You work as an analyst for the telecom operator **Megaline**. The company offers its clients two prepaid plans, Surf and Ultimate. The commercial department wants to know which of the plans is more profitable in order to adjust the advertising budget.

You are going to carry out a preliminary analysis of the plans based on a relatively small client selection. You'll have the data on 500 Megaline clients: who the clients are, where they're from, which plan they use, and the number of calls they made and text messages they sent in 2018. Your job is to analyze clients' behavior and determine which prepaid plan is more profitable.

**Skills Used: Statistical Data Analysis**

### Conclusion

As an analyst for Megaline, I was given data for 500 users acquired in 2018 and their activity that same year and tasked with **two objectives** as follows:

* Analyze client behavior
* Answer "which prepaid plan is more profitable?". Megaline will adjust advertising budget accordingly

Below are **INSIGHTS** discovered regarding **client behavior**:
* Surf and Ultimate users utilize the services similarly despite having different coverage. 
* Surf and Ultimate users churn at the same rate (6.8%), but surf users churn more quickly (about 2 months earlier)
* The Surf plan is more popular. 68% users are on the Surf plan and 32% on the Ultimate plan.
* Ultimate users under-utilize the services included and are very unlikely to incur extra fees (only 3% ultimate users go over their internet usage)
* Surf users are more likely to incur extra fees in internet (over 56% surf users) than either calls (35% of surf users) or messages (24% of surf users). Overall, 72% surf users have incurred extra fees.
* Surf users tend to be very cognizant of their limits as most users' monthly activity hover around it (sometimes unsuccessfully), particularly on call and internet service 
* Users tend to use call and internet service (used by 96% and 97% users respectively) but less likely to use messages with 20% users who have never used message service. 
* As internet is the only service type both users go over, Megaline is best positioned to make revenue from internet fees.
* As inquired, there is no evidence proving there is a statistically significant difference in the monthly profit between users from the NY-NJ region compared to users from other regions

**ANSWER: WHICH PREPAID PLAN IS MORE PROFITABLE?**

**The ultimate plan is more profitable for Megaline than the surf plan**. Although surf users are much more likely to incur extra fees (72% percent vs 3% for ultimate), these fees around 30 USD are much less than the 50 USD extra in monthly charge ultimate users pay. Hence, marketing should push the ultimate plan in favor of the surf plan.

**PROJECT LIMITATION(S)**:
* This study only looks at customers acquired in 2018 and their activity by the end of the calendar year they joined (12/31/2018). Hence, I had more data on customers the earlier they joined in the year. If there is reason to suspect the month the customer signed up has an effect on behavior, more research is advised.  


**ADDITIONAL BUSINESS RECOMMENDATIONS**
* Megaline is currently collecting a strange mix of city and regions for each user which is stored in the **'city' field**. It would be much easier to parse through if Megaline had a city and state fields. Regions could easily be formed combining the states. Why is this important? For example, Megaline had an interest in the NY-NJ region but the current region set up includes PA so I was forced to include PA data in the analysis. The separate fields would have solved this.
* 19% calls had a duration of **0 minutes** and 13% internet sessions used **0 MB**. Megaline should look into why as there is possiblity of lost revenue. Is this an intentional action from the customer to save on fees? An alternative to solve would be to charge a **connection fee** in which these 0 value calls and internet sessions would yield revenue. 
* Although churn rate is the same for both, the fact that **surf users churn much more quickly is something of concern**. Here, we looked at monthly revenue but surf users tend to 2 less months as a customer than ultimate users. 2 less months of monthly charge and fees. Megaline should consider an initiative to improve this metric (perhaps consider a third tier in the middle?). 

### Technologies Used

* Python (Pandas, Numpy, MatPlotLib, Seaborn, Scipy)

