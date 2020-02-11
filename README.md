# Sales-Target-Account-Dashboard
Various SQL code and dashboards I created for real applications at Periscope

#Background
On my sales team, we have a concept of "target accounts". 
These are a specific set of accounts that we as Account Executives (AEs) select to try to get meetings with.
The accounts come from a much larger list from an Account Development Representative that we work with.
Salesforce is our CRM, and a key purpose of Salesforce is to store and track the activities that we perform 
(emails, calls, etc.) on various accounts and contacts in the system. 
Activities on target accounts are one of several kinds of activities AEs perform each day.

#Problem
Because there are activities related to active evaluation, 
it is important to separate out activity focused on target account prospecting to get a clear picture
of the volume and focus of that activity. 
It occurred to me that there are several different ways of slicing those metrics that I would like to see all in one dashboard.
Another opportunity here is to put in that same place a method for identifying and selecting new accounts. 
The reason for that is that when this dashboard highlights that a certain account has received a lot of 
activity over a given time period, it indicates that it is likely time for that account to no longer be a target.
That means that it is time to find a different account to take it's place. 
Finding a new account can take time because there are thousands of accounts to choose from. 
With this explanation, this dashboard has three main goals:
  1.) Track activity on target accounts across the day, week, and month to know where we stand and to provide accountability
  2.) Survey the amount of activity across individual accounts to identify which accounts have been worked enough over
      a particular time horizon such that it's time to find a new account to focus on
  3.) In this same workspace, create an optimal way of identifying which accounts that are available to work are best to focus on now
  
#Solution
1.) Created three charts to track daily, and weekly activity on target accounts. The daily activity chart was created in the form of a number overlay chart, the weekly activity was created in the form of a horizontal bar chart to compare activity per week, and a third chart shows the daily activity by account for the day.
2.) Created a table chart that shows weekly, monthly, and quarterly per account, along with an account quality score. This is used to track activity across accounts over the given time period to determine when an account has been worked adequately, and to continually evaluate the quality of accounts being worked. This is the core tool for determining when to rotate out accounts.
3.) Created a table chart that shows key firmographic information about various accounts available in the system to be added to the target account list. I used several factors to give each account a score based on the number of those factors they possessed. Those factors were: Number of previous opportunities on the account, recency of funding, firm size, existence of employees who were previous users of Periscope, and company industry. 
