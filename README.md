# CUSTOMER COMPLAINTS MANAGEMENT AND RESPONSE ANALYSIS USING PYTHON AND POWERBI

________________________________________


## TABLE OF CONTENT 
- [BACKGROUND](#background)
-  [OBJECTIVES](#objectives)
- [DATA STRUCTURE AND INITIAL CHECKS](#data-structure-and-initial-checks)
- [EXECUTIVE SUMMARY](#executive-summary)
  -  [OVERVIEW OF FINDINGS ](#overview-of-findings)
- [INSIGHTS DEEP DIVE](#insights-deep-dive)
- [RECOMMENDATIONS](#recommendations)
-  [ASSUMPTIONS AND CAVEATS](#assumptions-and-caveats)
  

________________________________________
## BACKGROUND

Cumulus Financial Services founded in 1985 operates in the financial services industry, offering retail banking, asset management, corporate banking, and residential mortgage solutions. Active for several decades, Cumulus serves over 6 million customers across 59 states and the District of Columbia. Their business model integrates tailored financial products with digital convenience, supported by 2,700 branches and 8,600 ATMs. Key metrics include a $110 billion residential mortgage portfolio and recognition as a top middle-market loan syndicator for five consecutive years. They cater to diverse clients, including Fortune 500 companies, small businesses, and individuals, emphasizing innovation and customer-centric solutions.

Cumulus Financials’ dataset of customer financial complaints provide a unique opportunity to investigate the nature of customer grievances, company responses, and the efficiency of resolutions but despite having a comprehensive complaint database, identifying actionable insights to optimize complaint resolution and customer advocacy remains a challenge.

This report examines customer financial complaints to uncover trends in customer grievances, company responses, and operational efficiency. Data visualization and analysis techniques were used to identify key factors affecting complaint resolution and customer satisfaction. These findings aim to guide strategic improvements in customer advocacy and service delivery.

________________________________________

## OBJECTIVES

Insights with accompanying recommendations are provided in the outlined key areas below:
-	Customer complaints trends: Evaluating the trends of customer complaints across products and the states they were reported.
-	Submission channels analysis:  Analysed customer preferences by where they submit their complaints 
-	Company response effectiveness: An analysis of the success levels of customer relations at resolving issues effectively.
-	Month over month trend analysis: An evaluation on the volume of complaints trends and pattern by months 
-	Complaints quarterly trend: Assessment of the psychology underpinning trends in customer complaints on a quarterly basis.
-	Response timeliness over available submission channels: This is an assessment of the company’s effectiveness at handling complaints and how quickly they do so on an average.
-	Customer dispute pattern over time: An assessment to determine how customers disputed the company responses over time.
-	Customer disputes on resolutions evaluation: An evaluation of whether customers were satisfied with how their complaints were handled

________________________________________

The data used in this analysis was sourced from Cumulus Financial Internal database [HERE](https://drive.google.com/drive/folders/1nWtgRptXPwEicRi3-ALwlew7bCYQwsIm?usp=sharing)

The python script used to clean, format and normalize the data for this analysis can be found [HERE](https://github.com/paschaldubem/CUSTOMER-COMPLAINTS-MANAGEMENT-AND-RESPONSE-ANALYSIS/blob/main/TD_%20python_script.ipynb)

The interactive dynamic Powerbi dashboards used to report and explore trends in customer complaints and operational bottlenecks can be found [HERE](https://app.powerbi.com/view?r=eyJrIjoiYmZlMDU1YWItMjJkYS00MmNmLTk3MDMtNmZjZjE5YjgwZmFiIiwidCI6IjI5ZTg2YjVlLTVkMDctNGExNC1hZDQ0LWFiOTQ3NmUwZGE4NyJ9)
________________________________________


## DATA STRUCTURE AND INITIAL CHECKS 

Cumulus Financial services’ database structure seen below, consists of a single table with a total of 75,000 rows and 17 unique columns containing records spanning 2011 – 2020. 

![CUMULUS FINANCIAL CUSTOMER COMPLAINTS MANAGEMENT AND RESPONSE ANALYSIS spreadsheet snapshot ](https://github.com/user-attachments/assets/09cb883b-57bc-4a01-b186-5253cddac5de)



-	Complaint ID: Unique identifier for each complaint
-	Date Submitted: Date when the complaint was submitted
-	Product: Financial product associated with the complaint
-	Sub-product: Subcategory of the financial product
-	Issue: Description of the issue reported by the customer
-	Sub-issue: Additional detail about the issue
-	Company public response: The company's public-facing response to the complaint
-	Company: The company involved in the complaint
-	State: State from which the complaint was submitted
-	ZIP code: ZIP code of the complainant
-	Tags: Metadata about the complaint (e.g., related to elder customers, military, etc.)
-	Customer consent provided: Indicates whether the customer gave consent for data sharing
-	Submitted via: Channel used to submit the complaint (e.g., Web, Referral)
-	Date Received: Date when the complaint was received
-	Company response to Customer: The company’s response to the complaint 
-	Timely response: Indicates if the company responded within the required timeframe
	Customer disputed: Whether the customer disputed the company’s resolution

________________________________________

## EXECUTIVE SUMMARY
### OVERVIEW OF FINDINGS 

It was confirmed that credit cards and checking accounts product categories have been the primary sources of customer grievances with account management, deposits, and withdrawals emerging as the most frequent issues. 

Geographically, California, New York, and Florida recorded the highest complaint volumes, most likely a result of their high population densities; Additionally online submissions was the most utilized complaint channels, with web-based responses achieving the fastest resolution times and while 98.1% of the time these complaints were resolved timely, the insight remains tentative as gaps in dispute data particularly the 94.22% N/A responses from 2017-2020 underscore a need for improved data collection and reporting to ensure actionable insights. 

Below is an overview of a page from the powerbi dashboard, and more insights are included throughout the report. The dashboard can be viewed [HERE](https://app.powerbi.com/view?r=eyJrIjoiYmZlMDU1YWItMjJkYS00MmNmLTk3MDMtNmZjZjE5YjgwZmFiIiwidCI6IjI5ZTg2YjVlLTVkMDctNGExNC1hZDQ0LWFiOTQ3NmUwZGE4NyJ9)


![DASBOARD 1](https://github.com/user-attachments/assets/b73a06fa-3d5a-4520-818e-8b338a8413bb)

________________________________________


## INSIGHTS DEEP DIVE

### 1. CUSTOMER COMPLAINTS TREND

- BY GEOGRAPHICAL LOCATION (STATE) AND PRODUCT CATEGORIES

Cumulus Financial offers 7 products in over 60 states globally, and the concentration of customer complaints for each state and product was determined by the frequency of complaints reported within each state.

Further analysis of the complaint distribution across states revealed that California, New York, and Florida had the highest volumes of customer complaints, the elevated rates in these states could be attributed to several factors, like a high population density in these regions can correlate to a larger customer base, which increases the overall number of service interactions and, consequently, the likelihood of complaints. Additionally, a larger customer base often places greater strain on financial services resulting in delays, service disruptions, or other challenges that negatively affect the customer experience. 

On the product front, the analysis revealed that the credit card product had an overwhelming number (30k) of complaints reported by customers. This indicates that the credit card service was particularly problematic for users, suggesting a gap between customer expectations and the actual service experience. Customers who reported issues with the credit card service encountered difficulties related to various aspects of the product, such as account management, billing issues, or transaction processing problems. The high volume of complaints in this category signals that the credit card product would require targeted improvements to enhance its usability and address the pain points reported by customers.

The combination of regional factors, such as population density, and specific product-related issues, such as those with the credit card offering, highlights the areas where Cumulus Financial should focus its attention. Addressing these concerns could help reduce complaint volumes, improve customer satisfaction, and ensure that the company’s services are effectively meeting the needs of its diverse customer base across different states.

![image](https://github.com/user-attachments/assets/cbd32798-5080-4bc0-b08d-36898cf14876)


![image](https://github.com/user-attachments/assets/11252017-3348-40ca-b941-183ccfdf4fae)


### 2. BY ISSUES REPORTED 

In this analysis, findings indicated that the primary area of concern for Cumulus Financial customers was related to services involving account management (8.9k complaints), deposits and withdrawals (6k complaints). These categories accounted for majority of the reported issues. 
Further analysis revealed that the credit card product emerged as the most challenging for customers to manage, with account management being the most frequently reported issue within this product category. 
This suggests that customers encountered significant difficulties when interacting with the credit card service, particularly in relation to account management processes.

![Screenshot 2024-12-21 223959](https://github.com/user-attachments/assets/c4519815-430a-41d8-aae9-f94c92c8401c)


### 3. SUBMISSION CHANNELS ANALYSIS

It was revealed that the Web channel was the preferred medium for receiving complaints, accounting for 50.37% of all submissions. This highlights the Web as the most accessible medium for customers, likely due to its ease of use, 24/7 availability, and widespread adoption of digital technology. 

29.52% of complaints were submitted via referrals, indicating a significant reliance on third-party or directed assistance.

11.57% of complaints were lodged via phone calls, highlighting its continued relevance for customers who may prefer direct communication.

Postal mail and fax mediums accounted for just 7.05% and less than 2% respectively of complaints received, also indicating a phasing out of traditional methods in favour digital technology.

In contrast, Emails submissions recorded the lowest number of complaints, signifying minimal usage. This may suggest that customers find other digital options, such as the web interface, more convenient and responsive, reducing the appeal of email-based complaint submissions.

![image](https://github.com/user-attachments/assets/ffe67b93-fb48-406e-a736-c343eafbbebe)


### 4.	COMPANY RESPONSE EFFECTIVENESS

The high percentage of timely responses (98%) aligns with the organizational focus on enhancing customer satisfaction and operational excellence and showcases a strong focus on efficiency and customer service. Efficient response times are a critical driver of customer loyalty and help reduce the likelihood of churn or repeat complaints.

Only 1.95% of complaints were not addressed in a timely manner. While this is a minimal percentage, it highlights a potential opportunity to achieve near-perfect response rates by addressing any operational inefficiencies or bottlenecks.

![image](https://github.com/user-attachments/assets/1522db36-7b47-4454-bb5f-501562a19470)


### 5.	MONTH OVER MONTH TREND ANALYSIS 

In-depth analysis revealed the frequency of customer complaints exhibits a clear seasonal pattern. Complaints began relatively low at 5.7k in January and increased steadily to a peak of 7.1k in May. January to May sees a 24.5% increase in complaints, likely driven by post-holiday financial challenges or product/service issues surfacing early in the year.

After May, the volume stabilizes around 6.9K - 6.8K through June, July, and August, indicating a plateau during mid-year; June to August suggests consistent complaint levels, potentially indicating operational bottlenecks or recurring issues. 

A significant decline begins in September, continuing through November, where complaints reach a yearly low of 5.2K; September to November suggests seasonal resolution improvements or reduced customer activity.

In December, complaints slightly rebound to 5.4K. This may be linked to end-of-year financial product usage or unresolved holiday-related grievances.

![image](https://github.com/user-attachments/assets/003cb979-6190-4596-92e7-1aa2056dc3e8)


### 6.	COMPLAINTS QUARTERLY TREND

The quarterly trends in complaints represent the cumulative total of all complaint data from the 2011 to 2020, captured in the dataset. This aggregated approach provides a comprehensive view of customer behaviour and complaint patterns over the years, eliminating the potential for year-to-year anomalies to skew insights.

Q1 started with a relatively moderate complaint count of 18.1K, which gradually increased into Q2 and peaked in Q3. This upward trajectory highlights a period of increasing customer activity, possibly driven by emerging issues after the new year or delays in addressing residual concerns from the prior year.

Q3 recorded the highest volume of complaints at 20.6K, signalling consistent customer dissatisfaction or heightened activity in this period across multiple years. This peak could align with operational challenges, seasonal product/service demands, or mid-year financial reviews.

Q2 closely followed with 20.2K complaints, emphasizing the need for robust complaint resolution strategies in the middle of the year.

Q4 registered the lowest volume of complaints at 16.6K, a significant drop-off from the prior quarters. This reduction might be attributed to several factors:
-	Seasonal resolutions, as customers' concerns from earlier in the year are addressed.
-	Reduced customer activity with financial or service-related products as the year ends.
-	Improved operational efficiency towards the end of the year to address peak period backlogs.
  
By aggregating data from 2011 to 2020, the analysis eliminates outlier impacts and ensures that the trends represent recurring patterns rather than single-year anomalies. This comprehensive view provides strategic insights for long-term operational planning.

Decision-makers can leverage this visualization to align resources and refine processes to address high-complaint quarters more efficiently.

![image](https://github.com/user-attachments/assets/1909bcc7-b9c6-4d76-9ce0-d9145176595e)


### 7.	RESPONSE TIMELINESS OVER AVAILABLE SUBMISSION CHANNELS

The Web channel's rapid average response time of less than 2 days reflects the benefits of digital efficiency and automation which is likely driven by:
-	Automated systems that facilitate quick complaint acknowledgment and routing.
-	Integration of web submissions with customer relationship management (CRM) platforms, enabling faster action.
  
Web-based submissions may benefit from structured input fields, ensuring that complaints are logged with all necessary details upfront, reducing delays caused by back-and-forth communication.

On the flip side the email channel's poor response timeline of 6 days highlights the need for process improvements addressing these gaps will enhance overall customer satisfaction and streamline complaint handling.

This delay may be attributed to: 
-	Channels like Email might lack dedicated teams or automated triage systems, contributing to longer handling times compared to streamlined web-based platforms.
-	A slow integration of the technology into the system causing friction.

![image](https://github.com/user-attachments/assets/4b204575-3458-467c-87ce-2da264b0ef16)


### 8.	CUSTOMER DISPUTE PATTERN OVER TIME 

The analysis reveals a stark contrast between the year periods of 2011-2016 and 2017-2020 due to a staggering 94.22% missing responses in the latter period compared to 0% in the former. While earlier data (2011-2016) suggests meaningful patterns like the healthy percentage of Undisputed Responses (No) at 80.45%, the reliability of 2017-2020 dispute trends is limited necessitating further investigation to fully understand the challenges in maintaining data integrity in recent years, thus, making it difficult to reliably compare dispute trends between the two periods.

Disputed responses decreased from 19.55% (2011-2016) to only 0.68% (2017-2020). However, this sharp decline must be interpreted cautiously given the dominance of missing values.

The high percentage of missing responses (94.22%) in 2017-2020 could be due to system limitations, process changes, or a lack of emphasis on capturing dispute data.  The absence of incomplete records in 2011-2016 suggests that earlier periods had more robust data collection practices.

![image](https://github.com/user-attachments/assets/ebcfceac-d423-49e5-b617-9297a9e0dd22)
![image](https://github.com/user-attachments/assets/d9e64d88-1243-4e94-96a6-75057f1c6979)


### 9.	CUSTOMER DISPUTES ON RESOLUTIONS EVALUATION 

The analysis reveals that a majority of customer complaints were resolved without dispute, demonstrating a relatively high degree of customer satisfaction to company resolutions. However, the presence of a significant proportion of missing values highlights potential gaps in data collection warranting further investigation to ensure completeness and reliability of the insights.

Out of the total responses, 20K complaints were resolved by the company releasing a form of explanation without dispute, a substantial portion of the outcomes.
Conversely, 6k of company responses were still disputed by customers, indicating that 22.3% of Cumulus financials’ responses to solve these cases resulted in dissatisfaction from the customer's perspective.

The missing category accounts for 28.6K responses, which is 42.5% of all cases analysed. This is a significant proportion that cannot be ignored, as it likely represents instances where disputes were either not tracked, not applicable, or not recorded.

![image](https://github.com/user-attachments/assets/6351b32f-20fb-4679-8f84-1d9219464750)

________________________________________

## RECOMMENDATIONS

Based on the insights and findings outline, we would recommend decision makers to consider the following:

-	Based on the uncovered monthly trends, Optimizing Complaint Management During Key Periods to strengthen customer support and operational readiness during high-complaint periods, particularly from March to May, by analysing product types and issues reported during these peak months to identify common pain points. Additionally, focus on enhancing resolution processes before December to mitigate year-end issues and reduce future spillover complaints.
  
-	Available Submission mediums are key channels connecting us to our customers, so therefore Optimizing and Streamlining Complaint Submission Channels by enhancing the email submission process with user-friendly interfaces, tracking systems to improve its digital efficiency and encourage more use because emails are overall more cost effective and has greater reach. Strengthen phone-based support to meet the needs of customers preferring direct interaction, ensuring high satisfaction rates. Strategically downsize the use of dated channels, such as fax, to improve cost-efficiency while maintaining accessibility for specific demographics. Additionally, analyze referral data to understand its impact and identify opportunities for strategic partnerships or process improvements.
  
-	Responding to customers on time is a core strength so Sustaining such Timely Response Excellence is equally crucial by ensuring adequate staffing, implementing automation tools, and maintaining effective workflows in customer support operations. Address the 1.95% gap in delayed responses by investigating specific complaint types, submission channels, or operational bottlenecks, and implement targeted solutions to approach a 100% timely response rate. Regularly monitor performance trends using tracking tools to identify areas for further improvements, such as additional training, enhanced resources, or upgraded technology.
  
-	The average response time was 3 days across all submission channels but with a substantial range between the channels with the best (Web - average of 1 day) and least (Email – Average of 6 days) response times; a need to Optimize Complaint Resolution Across Submission Channels; enhance email efficiency by implementing automation tools for prioritization and categorization while training staff to accelerate complaint processing. Maintain web channel efficiency by continuing investments in CRM systems and ensuring robust IT infrastructure to manage growing volumes. Standardize operational workflows across all channels to provide a consistent customer experience and minimize disparities in response times.
  
-	Develop an action Plan to Address Data Gaps by conducting a thorough audit of missing responses to identify the root causes of missing dispute data (94.22% of dispute data from 2017-2020 was marked as missing), identifying whether the cause is technical, procedural, or systemic, and use these insights to improve future data collection. Enhance the data tracking framework to ensure all complaints have complete and accurate records, improving the reliability of future analyses.

________________________________________

## ASSUMPTIONS AND CAVEATS 

Assumptions were made throughout the analysis to adequately manage the challenges encountered with the data. These caveats are noted below

-	Approximately 49% of the data in the Customer Disputed column was identified missing posing a significant risk of skewing the analysis. Further investigation revealed that these missing values were exclusively from records spanning 2017–2020. To ensure accuracy and precision, the complete dataset was analyzed separately, isolating the affected records to minimize any potential bias.













  















