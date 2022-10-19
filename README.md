# nxtwave_sample_dataset
# Sample Dataset (part of assignment/recruitment) -TLDR


Kaggle Dataset link: https://www.kaggle.com/datasets/nxtwaveda/data-analyst

# Assignment
Assume you are a Data Analyst in an EdTech company. Your company is focused on accelerating its growth by increasing the number of enrolled users.

Therefore, you have been asked to analyze various aspects of customer acquisition to see the status of new users’ growth in your company. The insights you discover will help your business team in designing a better marketing strategy for your company.

# Expected Outcome
Brainstorm and identify the right metrics and frame proper questions for analysis. Your analysis should help your

- Business team to understand the lead's journey and stages with scope for improvement
- Business heads to understand their team performance
- Managers to understand their target areas

In case you identify any outliers in the data set, make a note of them and exclude them from your analysis.
Build the best suitable dashboard presenting your insights.

Your recommendations must be backed by data insights and professional visualizations to help your business team design road maps, strategies, and action items to achieve their goals.

Sales Business Dashboard: https://public.tableau.com/views/AssignmentBusinessDashboard/Dashboard1?:language=en-US&:display_count=n&:origin=viz_share_link

Manager Performance Dashboard: https://public.tableau.com/views/AssignmentPerformanceDashboard/Dashboard2?:language=en-US&:display_count=n&:origin=viz_share_link

Flowchart of leads conversion /internal hierarchy:
![image](https://user-images.githubusercontent.com/6307592/195079362-40296e30-a56b-4777-a004-fd8f81a4b824.png)



# Detailed Approach

## Understanding Datasets:

lead_basic_details: Contains details of the leads.
![image](https://user-images.githubusercontent.com/6307592/195073810-0707332d-b591-4215-ac30-dcc986623a67.png)


sales_managers_assigned_leads_details: Contains the details of the senior and junior sales managers and their assigned leads.

Each senior sales manager is assigned to 4 junior sales managers.

Each junior sales manager is assigned few leads in each cycle (a cycle is approximately a week).


![image](https://user-images.githubusercontent.com/6307592/195074159-e297be78-10ca-451f-aa95-10c07300c24c.png)


leads_interaction_details: Contains the details of call interactions of junior sales managers with the leads.
A lead can drop out at any stage of the flow. If there is no call by the junior sales manager to the lead after a certain stage then the lead is considered as dropped at that stage.

![image](https://user-images.githubusercontent.com/6307592/195074063-de85d9ad-440d-42b8-896c-088c45758f68.png)


leads_demo_watched_details: Contains the details of the demo session watched by the leads.

![image](https://user-images.githubusercontent.com/6307592/195073887-a063ebe0-ebe0-4754-9c9d-3a652c2c597c.png)


leads_reasons_for_no_interest: Contains the details of the reasons given by the leads for their lack of interest.

![image](https://user-images.githubusercontent.com/6307592/195074126-0d39b840-3c99-4c7b-aec5-457fffd1deab.png)


## Cleaning Datasets

To clean the datasets, i tried to find outliers and typos in the dataset. Once found, would proceed to remove the records or update them depending on the posibility.

![image](https://user-images.githubusercontent.com/6307592/195076760-9af99239-e053-4000-804b-9a1182ec4083.png)
![image](https://user-images.githubusercontent.com/6307592/195076879-94732495-57bf-41a3-bb73-fc7ac4eb46b8.png)

Once these records were removed, their primary keys ( forriegn keys ) were also removed from other datasets

There were also typos in datasets that i changed in excel/sheets directly.


## Analysing Datasets (BUSINESS/SALES) - refer flowchart above

##### In terms of leads details: 

We had to understand how many female and male leads were interested. 

![image](https://user-images.githubusercontent.com/6307592/195077409-dab07c84-f229-4b85-a486-44349e8fd8ac.png)

Then we had to understand which channel was bringing in the most leads.

![image](https://user-images.githubusercontent.com/6307592/195077587-b976506c-c89a-434d-b0c2-b50dcd11098f.png)

We also needed to understand their locations.

![image](https://user-images.githubusercontent.com/6307592/195077721-bf3a6b8d-9f65-4864-b27f-0f7ffa369820.png)

The findings of the dataset told us:

1. Hyderabad , Visakhapatnam and Kochi have higher number of students interested.
2. Leads from 'BTech' and 'Looking for job' are more likly to be interested.
3. Age group of leads ranges from 16 to 25.
4. Female leads are more likely to be interested compared to male leads.
5. Leads from Social media are more compared to other Means.

##### In terms of leads demo details: 

The language in which most leads preferred to watch demos.

![image](https://user-images.githubusercontent.com/6307592/195078406-e5785d0b-f638-447a-8287-3afb7aa662be.png)

And what was the breakdown of % demo watched.

![image](https://user-images.githubusercontent.com/6307592/195078709-d97b4655-041e-4c26-bb77-52d8d5bb4108.png)

##### The findings of the dataset told us:

1. English is the most prefered language to watch with, followed by Telugu and Hindi.
2. The chance of a lead watching 50% or more of the media is higher.

##### In terms of lead interactions merged with leads demo details:

Understand the languages preferred by the leads at different lead conversion stages.
![image](https://user-images.githubusercontent.com/6307592/195079560-b22645c3-3bce-4b53-a539-92196aa60da4.png)
![image](https://user-images.githubusercontent.com/6307592/195079607-143cb7a2-e870-4976-ac57-2b4701b19ad0.png)
![image](https://user-images.githubusercontent.com/6307592/195079674-ed1654e7-b3a1-4669-ae0a-2c1ab76e9bb2.png)
![image](https://user-images.githubusercontent.com/6307592/195079807-c92044c9-c137-445b-b138-2c4539b71dac.png)
![image](https://user-images.githubusercontent.com/6307592/195079860-35e8cad4-9ead-4bef-a96b-b034224ed6b8.png)

##### The finds of the dataset told us:
1. Leads speaking English have a higher conversion rate, followed by Telugu and Hindi
2. Leads speaking English also have a higher interest rate in different stages of conversion (specially after demo and interested in conversation/conversion), followed by Telugu and Hindi
3. Leads speaking English also reject the proposal alot more than Telugu and Hindi speakers

##### In terms of leads reasons for no interest in different lead conversion stages (Important):

Reasons to not be interested in the demo.

![image](https://user-images.githubusercontent.com/6307592/195080264-2d41e54e-4db8-418a-93dc-728453c4a1cf.png)

Reasons to not consider.

![image](https://user-images.githubusercontent.com/6307592/195080474-864d7707-9c74-429b-bddc-86c77f409e02.png)

Reasons to not convert.

![image](https://user-images.githubusercontent.com/6307592/195080694-7ab346a0-fb3c-448a-b4bb-ce6ae5807e4c.png)

There could be a chance Can't afford ranks high in all the charts could be due to their parents occupation, 
to lets join the 2 datasets to observe closely

![image](https://user-images.githubusercontent.com/6307592/195080845-cb206f8d-4b62-436f-91ae-a821b578e380.png)
![image](https://user-images.githubusercontent.com/6307592/195080898-0114007f-ba58-40d4-8aac-11450e096596.png)
![image](https://user-images.githubusercontent.com/6307592/195080947-b2472450-920e-4e0a-9f67-abc4bbd0257b.png)

##### The findings of the dataset told us: 

1. The top 3 reasons across the import stages are Can't afford, Wants offline classes and Students not interested in domain (in that order).
2. The top 3 parent occupation which result in reason 'Can't afford' are mainly Government Employee, Business and IT Employee (in that order)

## Analysing Datasets (MANAGER PERFORMANCE/LEAD CONVERT RATE) - refer flowchart above.

##### In terms of manager sales details:

How many junior managers had leads and who were they reporting to.

![image](https://user-images.githubusercontent.com/6307592/195081386-69cef0da-3f77-4d8f-8d38-c2ce5d214f1d.png)

How many junior managers were successful in converting leads.

![image](https://user-images.githubusercontent.com/6307592/195081555-33631c75-585e-41d7-b01e-b819a5e1a05b.png)

##### The findins of the dataset told us:

1. JNR1001MG junior manager has the most leads(33), and hence the SNR501MG has the most number of leads(93) spread across the junior managers.
2. JNR1016MG junior manager has the most successful conversions (8)


# Conclusion and Sugestion
##### On the business side of things:

1. Female leads are more interested then male but not much disparity. So focus on both genders.
2 .Focus more on the top 3 city locations which is Hyderabad, Vishakapatnam and Kochi. These locations also have most English and Telugu speakers which are the 2 most prominent languages to engage with leads and show them materials in these languages
3. Spend more on Social Media, and Website advertising. The user base is already healthy as user referrals are very high.
4. Come out with dicount for leads whose parents are associated with Government jobs.
5. Broaden the domain knowledge to fit more leads and if possible, think of offline mode of knowledge transfer.

##### On the operations/sales side of things:

1.Combine the best junior managers who had the highest converted % under the top senior managers.

2.Rotate junior managers not meeting certain % goal
