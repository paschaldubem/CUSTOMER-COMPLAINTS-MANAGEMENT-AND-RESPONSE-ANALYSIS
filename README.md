# CUSTOMER COMPLAINTS MANAGEMENT AND RESPONSE ANALYSIS USING PYTHON AND POWERBI


________________________________________
## ABSTRACT 



![DASBOARD 1](https://github.com/user-attachments/assets/b73a06fa-3d5a-4520-818e-8b338a8413bb)







This report examines customer financial complaints to uncover trends in customer grievances, company responses, and operational efficiency. Using data visualization and analysis techniques, I identified key factors affecting complaint resolution and customer satisfaction. The findings aim to guide strategic improvements in customer advocacy and service delivery.
________________________________________

## TABLE OF CONTENT 
- [INTRODUCTION](#introduction)
  -  [Background](#background)
  -  [Problem Statement](#problem-statement)
  -  [Objectives](#objectives)
  -  [Data Source](#data-source) 
- [DATA DESCRIPTION](#data-description)
- [KEY PERFORMANCE INDICATORS](#key-performance-indicators)
- [METHODOLOGY](#methodology)
  -  [Data Cleaning](#data-cleaning)
  -  [Exploratory Data Analysis](#exploratory-data-analysis)
- [ANALYSIS](#analysis)
  -  [Insights Uncovered](#insights-uncovered)
  -  [Approach](#approach)
- [RESULTS](#results)
  -  [Summary of Findings](#summary-of-findings)
  -  [Visualization](#visualization)
 - [CONCLUSION](#conclusion)
  -  [Summary](#summary)
  -  [Recommendations](#recommendations)


## INTRODUCTION
### Background
Understanding customer complaints is essential for enhancing satisfaction and operational efficiency. Cumulus Financials’ dataset of customer financial complaints provide a unique opportunity to investigate the nature of customer grievances, company responses, and the efficiency of resolutions.
### Problem Statement
Despite having a comprehensive complaint database, identifying actionable insights to optimize complaint resolution and customer advocacy remains a challenge. The project addresses this gap by uncovering patterns and trends.
### Objectives
1.	Identify trends in customer complaints across products, reported issues and states.
2.	Evaluate the timeliness and effectiveness of company responses.
3.	Provide actionable recommendations to improve customer advocacy and service quality.
________________________________________
### Data Source 

The data used in this analysis was sourced from [Cumulus Financial Internal database](https://drive.google.com/drive/folders/1nWtgRptXPwEicRi3-ALwlew7bCYQwsIm?usp=sharing) for a TDI data analysis project.

## DATA DESCRIPTION
The dataset includes the following fields:
-  Complaint ID- Unique identifier for each complaint
-  Date Submitted- Date when the complaint was submitted
-  Product- Financial product associated with the complaint
-  Sub-product- Subcategory of the financial product
-  Issue- Description of the issue reported by the customer
-  Sub-issue- Additional detail about the issue
-  Company public response- The company's public-facing response to the complaint
-  Company- The company involved in the complaint
-  State- State from which the complaint was submitted
-  ZIP code- ZIP code of the complainant
-  Tags- Metadata about the complaint (e.g., related to elder customers, military, etc.)
-  Customer consent provided- Indicates whether the customer gave consent for data sharing
-  Submitted via- Channel used to submit the complaint (e.g., Web, Referral)
-  Date Received- Date when the complaint was received
-  Company response to Customer- The company’s response to the complaint 
-  Timely response- Indicates if the company responded within the required timeframe
-  Customer disputed- Whether the customer disputed the company’s resolution
________________________________________

## KEY PERFORMANCE INDICATORS
-  Total Number of Complaints (75,513):

![Screenshot 2024-12-29 225531](https://github.com/user-attachments/assets/0c20080f-e8cb-471d-81b0-cce170b61c3f)

The analysis of the financial customer complaint dataset reveals that I have a total of 75,513 complaints. This significant number underscores the volume of customer dissatisfaction and the critical need for effective complaint management and resolution strategies.
  
-  Total Number of State (62):
  
![Screenshot 2024-12-29 225555](https://github.com/user-attachments/assets/2de0f46b-e495-4018-af7d-add23bd1a29e)

Our analysis reveals that customer complaints have been recorded from a total of 62 states. By examining complaint patterns and trends across these states, I can identify regional disparities, tailor our responses to specific areas, and implement targeted strategies to enhance customer satisfaction worldwide.

-  Total Number of Product (7):
  
![Screenshot 2024-12-29 225730](https://github.com/user-attachments/assets/2683579a-ac35-4016-977c-529b9e2aae37)

Our analysis indicates that there are 7 distinct financial products in our dataset. These products encompass a wide range of financial services, each with its own unique set of customer complaints.

-  Average Response Days (2.64):

![Screenshot 2024-12-29 225615](https://github.com/user-attachments/assets/43bbaefa-e2ef-4a9e-87d9-17bbcb4661d5)

Our analysis shows that the average response time for addressing customer complaints is approx 3 days. This metric is crucial as it reflects the efficiency and responsiveness of our complaint resolution process. A swift response time is essential for maintaining customer trust and satisfaction.

## METHODOLOGY
### Data Cleaning

Conducted data cleaning using python [Click here](https://github.com/paschaldubem/CUSTOMER-COMPLAINTS-MANAGEMENT-AND-RESPONSE-ANALYSIS/blob/main/TD_%20python_script.ipynb) to view my code base 


### Exploratory Data Analysis
1.	Analyzed the distribution of complaints by product, months of the year and state.
2.	Investigated submission channels to determine customer preferences.
3.	Evaluated the proportion of timely responses and disputed resolutions.
________________________________________

## ANALYSIS
### Insights Uncovered

#### 1.	Top Issues reported by customers 

![Screenshot 2024-12-21 223959](https://github.com/user-attachments/assets/c4519815-430a-41d8-aae9-f94c92c8401c)



In this analysis, the reported issues were initially visualized by counting the number of unique complaint IDs, resulting in a total of 87 reported issues. To identify the most frequent issues, the dataset was filtered using the filter pane feature, specifically applying the "Top N" function to isolate the top 5 most frequent issues. These top 5 issues were then displayed in a bar chart to provide a clear visual representation of the most common complaints. The findings indicated that the primary area of concern for Cumulus Financial customers was related to services involving account management, deposits, and withdrawals. These categories accounted for majority of the reported issues. Further analysis revealed that the credit card product emerged as the most challenging for customers to manage, with account management being the most frequently reported issue within this product category. This suggests that customers encountered significant difficulties when interacting with the credit card service, particularly in relation to account management processes.

#### 2.	Complaint Volumes Analysis by State and Product.


![Screenshot 2024-12-29 225142](https://github.com/user-attachments/assets/b457c4f2-f193-4953-b3db-ee9cb0fd62bb)



![Screenshot 2024-12-29 225356](https://github.com/user-attachments/assets/41781a90-de63-4ad8-a88d-d3e74c4e6a2e)


This analysis provides valuable insights into the variation of customer complaints across different states and products offered by Cumulus Financial. The company offers seven products in over 60 states globally, and the concentration of customer complaints for each state-product combination was determined by calculating the frequency of complaints within each state.

The data was thoroughly cleaned to ensure both accuracy and consistency before proceeding with the analysis. To begin, the complaints were visualized by counting the number of complaint IDs, which resulted in a total of eight distinct products, each with an associated count of total complaints.

To identify the top 5 products with the highest volume of complaints, the "Top N" feature in the filter pane was used to isolate these products. This enabled a focused analysis on the most frequently reported issues.

Further analysis of the complaint distribution across states revealed that California, New York, and Florida had the highest volumes of customer complaints. The elevated complaint rates in these states could be attributed to several factors, particularly the high population density in these regions. High population density typically correlates with a larger customer base, which increases the overall number of service interactions and, consequently, the likelihood of complaints. Additionally, a larger customer base often places greater strain on financial services, which may result in delays, service disruptions, or other challenges that negatively affect the customer experience. In the case of Cumulus Financial, the concentration of complaints in these populous states suggests that the company may need to evaluate whether its operational capacity and service quality in these high-density regions are adequate to meet customer demands.

On the product front, the analysis revealed that the credit card product had an overwhelming number of complaints reported by customers. This indicates that the credit card service was particularly problematic for users, suggesting a significant gap between customer expectations and the actual service experience. Customers who reported issues with the credit card service likely encountered difficulties related to various aspects of the product, such as account management, billing issues, or transaction processing problems. The high volume of complaints in this category signals that the credit card product may require targeted improvements to enhance its usability and address the pain points reported by customers.

The combination of regional factors, such as population density, and specific product-related issues, such as those with the credit card offering, highlights the areas where Cumulus Financial should focus its attention. Addressing these concerns could help reduce complaint volumes, improve customer satisfaction, and ensure that the company’s services are effectively meeting the needs of its diverse customer base across different states.

#### 3.	Most Utilized Submission Channels for Customer Complaints

![Screenshot 2024-12-29 225446](https://github.com/user-attachments/assets/5fdf463c-dc71-4492-97db-1db222cdc9fa)

The pie chart effectively illustrated the breakdown of complaints by channel, providing a straightforward visual representation of the relative proportions. By visualizing the data: I could easily identify which channels are most and least utilized. The insights supported a deeper understanding of customer behaviour and preferences for submitting complaints. 

The analysis revealed that the Web channel received the highest volume of complaints, accounting for 50.37% of all submissions. This highlights the Web as the most preferred and accessible medium for customers, likely due to its ease of use, 24/7 availability, and widespread adoption of digital technology. 

29.52% of complaints were submitted via referrals, indicating a significant reliance on third-party or directed assistance.

11.57% of complaints were lodged via phone calls, showcasing its continued relevance for customers who may prefer direct communication.

Postal mail accounted for 7.05% of complaints, indicating its reduced but steady usage among a specific demographic that prefers traditional methods.

Fax submissions were minimal, representing less than 2%, which underscores the decline in preference for the channel in favour of digital or direct interaction.

In contrast, Email submissions recorded the lowest number of complaints, signifying minimal usage. This may suggest that customers find other digital options, such as the web interface, more convenient and responsive, reducing the appeal of email-based complaint submissions. Streamlining or integrating email submissions into broader digital platforms could help consolidate resources while maintaining support for diverse customer needs.


#### 4.	Proportion of Complaints Resolved in a Timely Manner


![Screenshot 2024-12-29 231406](https://github.com/user-attachments/assets/52d0acaa-1bbd-448a-aed1-f6aa001ba798)


A pie chart was used to effectively convey the proportion of timely versus untimely responses, providing a clear visual snapshot of performance. This simple yet impactful representation underscores the organization’s overall success in achieving timely responses while also highlighting room for further optimization. By using a pie chart, I visualized the count of complaint ID by the timely response column.

The high percentage of timely responses aligns with the organizational focus on enhancing customer satisfaction and operational excellence. Efficient response times are a critical driver of customer loyalty and help reduce the likelihood of escalations or repeat complaints.

In the analysis, a significant 98.05% of complaints were addressed within a timely manner. This indicates that the majority of issues reported by customers were responded to promptly, showcasing a strong focus on efficiency and customer service.

Only 1.95% of complaints were not addressed in a timely manner. While this is a minimal percentage, it highlights a potential opportunity to achieve near-perfect response rates by addressing any operational inefficiencies or bottlenecks.

The pie chart clearly highlights the organization's overall success in responding to customer complaints in a timely manner. The 98.05% timely response rate reflects a well-executed strategy focused on operational efficiency and customer satisfaction. Addressing the minor gap in untimely responses through targeted improvements will further solidify the organization’s position as a leader in customer service excellence.


#### 5.	Monthly Trends in Complaint Volumes


![Screenshot 2024-12-29 225418](https://github.com/user-attachments/assets/ac957d6d-efc3-4a08-b863-dc442d556afc)


To effectively visualize the trends in customer complaints over a 12-month period, an area chart was employed, showcasing the fluctuations in complaint volumes month by month.

The analysis of the visualization reveals that the frequency of customer complaints exhibits a clear seasonal pattern. Complaints began relatively low at 5.7k in January and increased steadily to a peak of 7.1k in May. January to May sees a 24.5% increase in complaints, likely driven by post-holiday financial challenges or product/service issues surfacing early in the year.

After May, the volume stabilizes around 6.9K - 6.8K through June, July, and August, indicating a plateau during mid-year; June to August suggests consistent complaint levels, potentially indicating operational bottlenecks or recurring issues. 

A significant decline begins in September, continuing through November, where complaints reach a yearly low of 5.2K; September to November suggests seasonal resolution improvements or reduced customer engagement.

In December, complaints slightly rebound to 5.4K. This may be linked to end-of-year financial product usage or unresolved holiday-related grievances. 


#### 6.	Average Response Time by Submission Channels


![Screenshot 2024-12-29 225807](https://github.com/user-attachments/assets/6c979943-e121-45ec-aa64-20d5688c73fa)



In this analysis, a tree map was used to effectively convey the proportion of average response time, providing a clear visual snapshot of performance. The Web channel's rapid average response time reflects the benefits of digital efficiency and automation, while the Email channel's slower response highlights the need for process improvements. Addressing these gaps will enhance overall customer satisfaction and streamline complaint handling.

Complaints submitted via Email had the slowest average response time at approximately 6 days. This delay may be attributed to: 

-  Channels like Email might lack dedicated teams or automated triage systems, contributing to longer handling times compared to streamlined web-based platforms.

-  The company is reluctant to integrate the technology into their system causing friction.
  
Complaints submitted through the Web channel had the fastest average response time of less than 2 days. This efficiency is likely driven by:

-  Automated systems that facilitate quick complaint acknowledgment and routing.
-  Integration of web submissions with customer relationship management (CRM) platforms, enabling faster action.
  
Web-based submissions may benefit from structured input fields, ensuring that complaints are logged with all necessary details upfront, reducing delays caused by back-and-forth communication.

#### 7.	Quarterly Comparison of Complaint Volumes Over the Years


![Screenshot 2024-12-29 230421](https://github.com/user-attachments/assets/bc66ea3e-998f-43a1-a96a-6ad5ffca49df)


The quarterly trends in complaints represent the cumulative total of all complaint data from the years 2011 to 2020, as captured in the dataset. This aggregated approach provides a comprehensive view of customer behaviour and complaint patterns over the years, eliminating the potential for year-to-year anomalies to skew insights.

Quarter 3 recorded the highest volume of complaints at 20.6K, signalling consistent customer dissatisfaction or heightened activity in this period across multiple years. This peak could align with operational challenges, seasonal product/service demands, or mid-year financial reviews.

Quarter 2 closely followed with 20.2K complaints, emphasizing the need for robust complaint resolution strategies in the middle of the year.

Quarter 4 registered the lowest volume of complaints at 16.6K, indicating a significant drop-off from the prior quarters. This reduction might be attributed to several factors:

-  Seasonal resolutions, as customers' concerns from earlier in the year are addressed.
-  Reduced customer engagement with financial or service-related products as the year ends.
-  Improved operational efficiency towards the end of the year to address peak period backlogs.
  
Quarter 1 started with a relatively moderate complaint count of 18.1K, which gradually increased into Quarter 2 and peaked in Quarter 3. This upward trajectory highlights a period of increasing customer activity, possibly driven by emerging issues after the new year or delays in addressing residual concerns from the prior year.

By aggregating data from 2011 to 2020, the analysis eliminates outlier impacts and ensures that the trends represent recurring patterns rather than single-year anomalies. This comprehensive view provides strategic insights for long-term operational planning.

The area chart effectively captures these cumulative trends, offering a clear visual representation of how complaint volumes fluctuate throughout the year. Decision-makers can leverage this visualization to align resources and refine processes to address high-complaint quarters more efficiently. I used an area chart to visualize the date received column by the count of complaint ID, and by default this gave us the complaint ID per year which I then drilled down to get the complaint ID per quarter.


#### 8.	Trends and Patterns in Customer Disputes Over Time


![Screenshot 2024-12-23 233015](https://github.com/user-attachments/assets/17e06228-fa34-43e0-ad56-7c8a1dbc5578)


![Screenshot 2024-12-23 233414](https://github.com/user-attachments/assets/14aad6dc-a8e9-44d9-b13d-a603815003d6)


The analysis reveals a stark contrast between 2011-2016 and 2017-2020 due to the overwhelming prevalence of N/A responses in the latter period. While the earlier data suggests meaningful patterns, the reliability of 2017-2020 dispute trends is limited, necessitating further investigation to fully understand the dynamics of customer disputes during this timeframe.

-  A staggering 94.22% of responses in 2017-2020 lack dispute data compared to 0% in 2011-2016. This suggests significant challenges in maintaining data integrity in recent years, making it difficult to reliably compare dispute trends between the two periods.
  
-  Disputed responses decreased from 19.55% (2011-2016) to only 0.68% (2017-2020). However, this sharp decline must be interpreted cautiously given the dominance of N/A values.
-  Reduction in Undisputed Responses (No) also dropped from 80.45% (2011-2016) to 5.1% (2017-2020). This further reflects the impact of the 94.22% N/A responses on the dataset, as the majority of responses lack dispute classification.
  
The high percentage of N/A responses (94.22%) in 2017-2020 highlights gaps in recording or reporting customer dispute information. This could be due to system limitations, process changes, or a lack of emphasis on capturing dispute data.  The steep decline in disputes and undisputed responses may not reflect actual improvements in customer satisfaction or company resolution processes but rather incomplete data for this period.  The absence of N/A values in 2011-2016 suggests that earlier periods had more robust data collection practices, whereas post-2016 processes appear less reliable.


#### 9.	Analysis of Customer Disputes on Company Responses


![Screenshot 2024-12-29 230933](https://github.com/user-attachments/assets/b6ef96b6-931d-4cda-a7e7-479e1323d669)



The analysis reveals that the majority of customer complaints were resolved without dispute, demonstrating a relatively high degree of customer satisfaction or acceptance of company resolutions. However, the presence of a significant proportion of N/A values highlights potential gaps in data collection or processing, warranting further investigation to ensure completeness and reliability of the insights.

Out of the total responses, 20.2K complaints were resolved without dispute, representing a substantial portion of the outcomes.

Conversely, 5.8K complaints were disputed by customers, indicating that 22.3% of resolved cases resulted in dissatisfaction or unresolved issues from the customer's perspective.

The N/A (Not Available) category accounts for 28.6K responses, which is 42.5% of all cases analyzed. This is a significant proportion that cannot be ignored, as it likely represents instances where disputes were either not tracked, not applicable, or inadequately recorded.

If some of these N/A responses are actually disputed cases, the overall dispute percentage could increase, potentially altering the narrative about customer satisfaction.

Disputes were more frequent for cases labelled as "Closed with Monetary Relief" and "Closed with Non-Monetary Relief," suggesting dissatisfaction with the type or adequacy of resolutions provided in these cases.

Closed with Explanation responses had the highest number of N/A entries. This may indicate inconsistencies in tracking dispute outcomes for cases resolved in this manner.

### Approach
-  Used Python and Power BI for data transformation and visualization.
-  Utilized key libraries like NumPy and Pandas, and power query to explore relationships among key variables.
-  Developed interactive dashboards for trends visualization.
  
## RESULTS
### Summary of Findings

1.	Majority of complaints stem from issues with credit cards and checking accounts.
2.	Online submissions dominate, suggesting the importance of optimizing digital submission processes.
3.	Timely responses correlate with higher customer satisfaction.
4.	The primary area of concern for Cumulus Financial customers are related to services involving account management, deposits, and withdrawals.
5.	 Complaint distribution across states revealed that California, New York, and Florida had the highest volumes of customer complaints.
6.	The analysis reveals that the frequency of customer complaints exhibits a clear seasonal pattern.
7.	 The Web channel's rapid average response time reflects the benefits of digital efficiency and automation, while the Email channel's slower response highlights the need for process improvements. 
8.	Quarter 3 recorded the highest volume of complaints at 20.6K, signalling consistent customer dissatisfaction or heightened activity in this period across multiple years. 
9.	A staggering 94.22% of responses in 2017-2020 lack dispute data compared to 0% in 2011-2016. This suggests significant challenges in maintaining data integrity in recent years which highlights gaps in recording or reporting customer dispute information. This could be due to system limitations, process changes, or a lack of emphasis on capturing dispute data. 
10.	Majority of customer complaints were resolved without dispute, demonstrating a relatively high degree of customer satisfaction or acceptance of company resolutions. However, the presence of a significant proportion of N/A values highlights potential gaps in data collection or processing, warranting further investigation to ensure completeness and reliability of the insights.

### Visualization

![DASBOARD 1](https://github.com/user-attachments/assets/e1c11289-8a14-4173-8354-c1c1f7e5e0a9)

![Screenshot 2024-12-29 232402](https://github.com/user-attachments/assets/0afc1883-5946-404c-bd4f-dca3403d68d9)

Dashboards include:
-  Complaint volumes by product, state, and year.
-  Trends in submission channel preferences.
-  Response efficiency metrics.
-  To access the interactive PowerBI dashboard [Click Here](https://app.powerbi.com/view?r=eyJrIjoiYmZlMDU1YWItMjJkYS00MmNmLTk3MDMtNmZjZjE5YjgwZmFiIiwidCI6IjI5ZTg2YjVlLTVkMDctNGExNC1hZDQ0LWFiOTQ3NmUwZGE4NyJ9)
________________________________________

## CONCLUSION

### Summary

This analysis provides actionable insights into financial complaint trends, highlighting areas for improvement in operational and advocacy strategies. The study highlights key trends and patterns in Cumulus Financials’ complaint management and resolution processes. Credit cards and checking accounts emerged as the primary sources of customer grievances, with account management, deposits, and withdrawals being the most frequent issues. Geographically, California, New York, and Florida recorded the highest complaint volumes, linked to population density. Online submissions dominated complaint channels, with web-based responses achieving the fastest resolution times. While 98.1% of complaints were resolved timely, gaps in dispute data particularly the 94.22% N/A responses from 2017-2020 underscore a need for improved data collection and reporting to ensure actionable insights.

### Recommendations

#### 1.	Optimize Complaint Management During Key Periods:

Strengthen customer support and operational readiness during high-complaint periods, particularly from March to May, by analyzing product types and issues reported during these peak months to identify common pain points. Additionally, focus on enhancing resolution processes before December to mitigate year-end issues and reduce future spillover complaints.

#### 2.	Optimize and Streamline Complaint Submission Channels: 

Enhance the web submission process with user-friendly interfaces, tracking systems, and prompt acknowledgment features to improve digital efficiency. Strengthen phone-based support to meet the needs of customers preferring direct interaction, ensuring high satisfaction rates. Strategically streamline lesser-used channels, such as fax, to improve cost-efficiency while maintaining accessibility for specific demographics. Additionally, analyze referral data to understand its impact and identify opportunities for strategic partnerships or process improvements.

#### 3.	Achieve and Sustain Timely Response Excellence: 

Prioritize timely responses by ensuring adequate staffing, implementing automation tools, and maintaining effective workflows in customer support operations. Address the 1.95% gap in delayed responses by investigating specific complaint types, submission channels, or operational bottlenecks, and implement targeted solutions to approach a 100% timely response rate. Regularly monitor performance trends using tracking tools to identify areas for further improvements, such as additional training, enhanced resources, or upgraded technology.

#### 4.	Optimize Complaint Resolution Across Submission Channels: 

Enhance email efficiency by implementing automation tools for prioritization and categorization while training staff to accelerate complaint processing. Maintain web channel efficiency by continuing investments in CRM systems and ensuring robust IT infrastructure to manage growing volumes. Standardize operational workflows across all channels to provide a consistent customer experience and minimize disparities in response times.

#### 5.	Action Plan to Address Data Gaps and Frequent Disputes: 

Conduct a thorough audit of N/A responses to identify the root causes of missing dispute data, uncovering patterns or operational gaps in the resolution process. Enhance the data tracking framework to ensure all complaints have complete and accurate records, improving the reliability of future analyses. Focus on cases involving monetary and non-monetary relief, addressing the underlying causes of higher dissatisfaction levels to improve overall customer resolution satisfaction.

#### 7.	Enhance Data Integrity and Customer Feedback Processes: 

Conduct a detailed review to understand why 94.22% of dispute data from 2017-2020 was marked as N/A, identifying whether the cause is technical, procedural, or systemic, and use these insights to improve future data collection. Implement uniform data collection standards to ensure consistency across all years and avoid gaps. Where possible, analyze annual trends separately to detect smaller patterns and better explain dispute trends. Additionally, investigate qualitative customer feedback from 2017-2020 to supplement the incomplete data and gain a deeper understanding of customer sentiment.
________________________________________

