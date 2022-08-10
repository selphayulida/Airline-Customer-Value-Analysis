# Airline Customer Value Analysis through LRFMC Indicators by Performing K-Means Clustering Algorithm

## Background
- Along with the development of information and technology accompanied by increasingly fierce business competition, the company is trying to shift from a product-centric approach to a customer-centric approach.
- A customer-centric approach will enable companies to create better relationships with customers, prioritize customer needs, and increase customer retention, which will lead to increased company profits.
- For this reason, companies need to classify customers accurately, formulate personalized service plans based on the classification results, and optimize enterprise marketing resource allocation plans.
- The aviation company's marketing team can establish a reasonable customer value evaluation model, segment customers, analyze and compare the value of customers from different groups, and formulate appropriate marketing strategies to provide personalized customer service according to customer needs.

## Objectives
Against this background, the main goal of this experiment is customer value analysis, which is to do customer clustering/ segmentation. One of the most popular, easy-to-use, and effective segmentation methods for identifying customer value is to segment customers through RFM indicators. But in this project we will extend the indicators to be LRFMC that will be explained later. This experiment analyzes customer information and airline flight records collected in 2014. Objectives of this experiment include:
- Perform customer segmentation (clustering) through the airline customer dataset. We use LRFMC indicators and perform K-Means clustering algorithm.
- Analysis of the characteristics of each cluster resulting from segmentation.
- Provide business insight related to the analysis results.

## The Steps
This dataset consists of 62988 rows and 23 columns. In this project, we will do airline customer value analysis through LRFMC indicators by performing K-Means clustering algorithm. The steps in this project include:
1. Data collection.
2. Data understanding by performing the statistic descriptive of data and check correlation among features by correlation matrix.
3. Data preprocessing that includes handling missing value, feature selection based on LRFMC, handling outlier and also data scaling.
4. Clustering process by K-Means algorithm
5. Analyze the result - customer value analysis

## Results
After selecting features based on LRFMC indicators as well as some preprocessing for clustering purposes with the K-Means algorithm, the customer segmentation results into 5 clusters (5 customer groups) are as follows:

![newplot](https://user-images.githubusercontent.com/105648751/183899447-6a328650-67a1-49e5-8e73-92a0d8bdd6af.png)

**1. Cluster 0 - Customer Group 1 :**
  - This is a group of customers who actually fly frequently, have a high monetary value because of their high mileage and are customers who have been in the frequent flyer program for a long time. The average discount rate is moderate. And this customer has a good recency because they recently flew with this airline.
  - Let's label this customer as **The Champions**.

**2. Cluster 1 - Customer Group 2 :**
  - This customer group is a new customer (recently joined the frequent flyer program) so it has an RFMC value that is not yet high but looks potential.
  - Let's label this customer as **Potential Loyalists - New Customers**.
  
**3. Cluster 2 - Customer Group 3 :**
  - This customer group is those who have been in the frequent flyer program for quite a while. However, this group actually does not use this airline very often, has a low monetary or mileage value and the average discount rate is also quite low. They also have not used this airline for a very long time.
  - Let's label this customer as **Hibernating - Low Value Customers**.

**4. Cluster 3 - Customer Group 4 :**
  - This customer group is a customer who has been in the frequent flyer program for a long time and has a moderate RFMC score. They don't fly very often just moderate, so the other values are also moderate but actually have potential.
  - Let's label this customer as Potential **Loyalists - General Customers**.
  
**5. Cluster 4 - Customer Group 5 :**
  - This customer group has been joining the frequent flyer program for a long time. They have not used this airline for a very long time and have high average discount rate. And this customer group rarely flies and has low monetary value or mileage.
  - Let's label this customer as **Hibernating - Price Sensitive Customers**.

## Business Recommendation
Business Recommendation based on Customer Value Analysis:
1. **The Champions** - Customer Group 1
    - Airline must really take care of this customer group, because this group contributes well to the business. They can become early adopters for new airline service or program, and will help promote it. One way to keep these customers is through a reward program for this type of customer group. The reward program can also be accompanied by a kind of referral program, with the aim of providing rewards but encouraging them to promote airline brands (or certain programs).
    - Example:
        - Special reward discount + post your flight experience for additional discount for the next flight
        - More FFP points (x2/x3) for your flight + booked your flight with friends and get special discount/price
        - Book 1 for 2 - just for you - and triples your point
        - Travelling - Chilling - Healing - Saving. Flying to our new route with xx% discount + triples your ffp point. Catch additional points!!! Get more when your friends booked this route with ur refferal code.
        - My Poin Rewards - Provides convenience and various point reedem options.
        - etc.
        
2. **Potential Loyalists - New Customers** - Customer Group 2
    - This customer has recently joined the ffp program at this airline. However, they have potential as loyal customers in the future, as can be seen from the good RFMC value as a new customer. By building a good relationship with onboarding support and special offer programs, it may be possible to help increase their frequency and mileage.
    - Example:
        - Flight Booking assistant
        - Boost your tier by special flight discount rate with us - double your mileage now
        - Friday escape with firends to upgrade your tier
        - etc.       
        
3. **Hibernating - Low Value Customers** - Customer Group 3
    - This customer has a fairly low value for the airline. There is a possibility that they are the type of customers who fly only because there are certain interests or events. Although the company is not obliged to focus on this type of customer, the company should still try to induce them otherwise they will be completely lost. Airline should make a program to wake them up from hibernation.
    - Example:
        - I miss u or I don't wanna lose you program. Give special discount or flight rate.
        - Can't forget u / Let's do it again/ Can't move on Program. Awake them with good memory of their last flight by giving them voucher/ code discount rate with flight routes according to their last flight.
        - etc.
      
4. **Potential Loyalists - General Customers** - Customer Group 4
    - This customer group is similar to group 2, but they have been in the frequent flyer program for longer. This customer has a pretty good track record but needs to be improved because they have the potential to contribute more to the company's business. The programs or campaigns that can be offered are more towards increasing engagement by telling them that they are loyalists (even though they are not champions) and influencing them to continue with us and create more shared moments.
    - Example:
        - Let's be our part forever - Give special rewards point for next booking
        - Fly more get more - doubles the points for this year (particular time period) booking
        - Share your moment with us - for additional points to boost your tier and discover the next treasure
        - etc.
    
5. **Hibernating - Price Sensitive Customers** - Customer Group 5
    - This customer is similar to group 3, only they seem to have a higher price sensitive. So the approach taken by the company must be more aggressive than group 3. Programs that can be provided to wake them up must be more thought-provoking with special prices or discounts and various benefits that are more attractive to them. The company can provide a typical special program with what they might have gotten before.
    - Example:
        - I want to get back together with you - This Deal is just for you
        - Don't you miss this Biggest Deal? Let's do it again!
        - etc.
 
## References
The following are references in working on this project.
- https://www.programmersought.com/article/63823799496/
- https://www.kaggle.com/code/felixign/airline-clustering/notebook
- https://www.kaggle.com/code/amarmaruf/homework-unsupervised-rakamin-ds8/notebook
- https://clevertap.com/blog/rfm-analysis/
- https://www.moengage.com/blog/rfm-analysis-using-rfm-segments/


**Please kindly note that the highlight of this project is performing K-Means clustering algorithm for customer value analysis through LRFMC indicators as part of my learning journey, so there may be some steps missed or not optimized yet. The Business insight and recommendation are also part of my learning journey, so maybe they are not as sharp, or as professional as the experts.**
