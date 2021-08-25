# **Top-Advertisers**


![Images](image1.jpeg)


Determine the top advertisers for each application and country.  Verve Data Engineering Challenge.


Authors: Esaa Yamini, Alex Nastetsky


# **Process**


Given two json files, make a recommendation for the top 5 advertisers to display for each app and country combination based on impressions, clicks, and revenue.


# **Analysis**


The impressions_json file had several duplicate UUIDs which skewed the data.  Removing duplicates reduced unique impressions to 66 events.  Merging impressions_json with the clicks_json (to analyze revenue per impression), further reduced the workable data to only 64 events.  Analysis of the cleaned data indicates there were no more than two top advertisers for any app_id / country_code combination (as shown in the "recommended_advertiser_id" json file).  Results will be significantly different if duplicate UUIDs are not dropped.  
