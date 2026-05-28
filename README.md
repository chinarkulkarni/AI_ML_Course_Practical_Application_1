# AI\_ML\_Course\_Practical\_Application\_1

This is a repository for the Practical Application 1 in Module 5 of Berkeley Haas AI/ML Course



1. Project Title: Will the Customer Accept the coupon?

   * This application reads the data from coupons.csv, and performs data cleanup, filtering and analysis, and provides observations made from the analysis.

2\. The link for the notebook file: https://github.com/chinarkulkarni/AI\_ML\_Course\_Practical\_Application\_1/blob/main/prompt.ipynb

3\. Data Overview:

   * The spreadsheet data/coupons.csv comes from the UCI Machine Learning repository, collected via a survey on Amazon Mechanical Turk.
   * It describes the different driving scenarios, and asks the person driving, whether he will accept the coupon presented.
   * The Y column provides his response (1 means either 'right away' or 'later before the coupon expires', and a 0 means 'I do not want the coupon'. 

3\. Data Analysis methodology:

   * The data is read, cleaned up and analyzed using the python libraries Pandas, Seaborn and NumPy.
   * Data cleanup for missing fields is done using fillna() and dropna() methods of the Pandas library.
   * Various Bar charts and Histograms are plotted to observe the trends of the Coupon Acceptance rates based on different parameters.
   * Further observations and calculations are done using the library's standard calculation methods to calculate the rates, find out the factors that affect the rates, and conclude which parameters and values result in higher acceptance rates for specific types of coupons.

4\. Here are the findings made during the data analysis:

   * Findings for the overall coupon acceptance rates:

     * The overall coupon acceptance rate is 57%.
     * Some coupons are more popular than others. The cheaper restaurant and Carry out and Take away coupons have a higher rate (\~70%) than the expensive restaurants and Bar coupons (\~40%)
     * Some factors like the Weather, temperature, time of day, destination, passenger, expiration do affect the coupon acceptance rates, while others like gender and whether they have children or not, do not have much of an impact on them.
     * Different coupon types are more popular among different age groups. (E.g. Coffee coupons more popular among younger age groups, while expensive restaurants are more popular among older groups)
     * The coupons of specific types are more popular among the people that visit the related establishments more frequently. This is true for all types of coupons except the Carry out ones, which are popular among all people regardless of the number of visits.
   * Findings for the Bar coupons:

     * The overall acceptance rate for Bar type coupons (41%) is lower than the other types, like the Carry out coupons (70%).
     * The acceptance rate is higher among those who visit the bars frequently
     * It is also higher among adults who visit the bar at least once
     * It is higher among people who are not widowed and are not driving with a kid as a passenger.
     * It is only slightly higher (than average) among people who visit cheaper restaurants frequently, and are in the lower income groups.
   * Findings for the Expensive Restaurant coupons:

     * The acceptance rate for expensive restaurants is lower than the average acceptance rates across all coupon types, but higher than the bar coupons.
     * It is higher for people who visit the expensive restaurants 4 or more times per month.
     * It is more popular among people who are single or divorced, and/or have kids.
     * The coupons that have a longer expiration date of 1 day have a higher acceptance rate than the short lived ones.



