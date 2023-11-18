# Youtube_Consumer_Usage_Analysis
CNIT 372 Project Fall 2023

Group #7 Milestone 1
Group Names: Kevin Patel, Nisarg Patel, Yug Vasani
Option Choice: Option A - Usage of YouTube as a Content Consumer
We plan to use the YouTube Statistics, Most Subscribed Youtube Channels, and Global YouTube Statistics 2023.
YouTube Statistics: This dataset includes a wide range of YouTube-related statistics, including counts for subscribers, views, likes, dislikes, comments, and other forms of involvement for different channels and videos. Additionally, it might contain details on the types of videos, upload rates, and other things.
Most Subscribed Youtube Channels: This dataset probably contains statistics on the top YouTube channels with the most subscribers. It might contain information like channel names, subscriber totals, video totals, and category counts.
Global YouTube Statistics 2023: This dataset appears to be a special collection of 2023 YouTube statistics, presumably encompassing global trends, usage trends, and performance measures.
The data set encompasses information about YouTube users, videos, channels, and global statistics. The insights derived from this data can help content creators, marketers, and businesses make informed decisions, optimize their content, and better understand their target audience and the YouTube platform's dynamics.
Database Design:
Table 1: Consumer
ConsumerID (PK, VARCHAR2(10)): Unique identifier for consumers
ConsumerName (VARCHAR2(50)): User's display name on YouTube
Age (NUMBER(3)): Consumer’s Age (Optional)
Gender (VARCHAR2(10)): Consumer’s Gender (Optional)
Location (VARCHAR2(50)): Consumer’s Location (Optional)
RegistrationID (DATE): The date when the user registered on YouTube
Table 2: YTVIDEO
VideoID (PK, CHAR(15)): Unique identifier for Video
Category (VARCHAR2 (30)): Category of YouTube video
Date (DATE): Date of upload
Likes (INTEGER): Number of likes on the video
Dislikes(INTEGER): Number of dislikes on the video
Comments(INTEGER): Number of comments on the video
Views (INTEGER): Number of Views on the video
Title( VARCHAR2(55)): Title of the video
Table 3. Channel 
ChannelName (PK, VARCHAR2 (60)): Name of the Channel
ChannelType (VARCHAR2(30)): Brief description of the Channel
SubscribersCount (INTEGER): Number of Subscribers of the Channel
Videos (INTEGER): Number of videos the Channel has
VideoViews (INTEGER): Number of views each Channel has
Country (CHAR): Name of the country where the owner of the Channel is from

Relationships: Consumer-< YTVIDEO | Consumer -< Channel | Channel -< YTVIDEO



Team Contribution:
The team chose this topic based on personal interest, project objectives, research, and inspiration.
Kevin Patel: Datasets, Database design, Brainstorming, Formatting, Planned relationships.
Yug Vasani: Brainstorming Datasets, Database Design, Formatting, Wrote relationships.
Nisarg Patel: Datasets, Brainstorming, Database design, Formatting, Planned relationships.


Group #2 Milestone 2 
Group Names: Kevin Patel, Nisarg Patel, Yug Vasani
Option Choice: Option A - Usage of YouTube as a Content Consumer
Question 1: What are the key demographic factors influencing customer satisfaction in our retail business?
Knowledge Used: To answer this issue, data analysis and statistical methods will be used to determine the main demographic variables that affect customer satisfaction in a retail business. Data about client demographics (such as age, gender, income, geography, etc.) and customer satisfaction levels may need to be gathered.
Importance/Usefulness: Understanding the key demographic factors that influence customer satisfaction is crucial for a retail business. It also helps marketing and sales teams target specific demographics for improved customer experience.
Question 2: What is the most common age range among consumers who have registered on YouTube in the last six months?
Knowledge Used: SQL date functions and data filtering.
Importance/Usefulness: This information can assist in tailoring content and advertising strategies to the age group most actively joining the platform, helping marketers and content creators stay relevant.
Question 3: Which channel type has the highest average number of video views per video?
Knowledge Used: SQL queries for calculating averages and sorting data.
Importance/Usefulness: This query can assist marketers and channel owners in determining which channel kinds are the most interesting, enabling them to invest resources wisely and enhance their content strategy.
Question 4: Are there any geographical areas with a high concentration of dissatisfied customers?
Knowledge Used: In order to discover geographic locations with a large proportion of unsatisfied consumers, this topic makes use of geographic data analysis, including mapping and data visualisation techniques. It necessitates having access to the relevant sites of customer satisfaction data. SQL Techniques: sorting, calculating maximum numbers, data filtering
Importance/Usefulness: Enables targeted customer support efforts in areas with lower satisfaction. By analyzing geographic patterns in customer satisfaction, youtubers can enhance their strategies, improve customer experiences, and ultimately drive better business outcomes.
Question 5: What percentage of the videos I watch are from channels I am subscribed to versus unsubscribed channels? 
Knowledge Used: Data analysis and database querying skills are required for this question. To gather information on the videos you have seen, determine which of them are from subscription channels, and determine the percentage based on this data, you would need to specifically query the database.
Importance/Usefulness: Individual users may find this information useful in understanding their watching interests and habits. It may show whether they are interacting more with channels they already subscribe to and find interesting or whether they are checking out content from fresh, unsubscribed channels. Also, this data can be used by content producers to evaluate the success of their subscription-based audience engagement. They can use it to monitor the proportion of their content that is consumed by subscribers versus non-subscribers, which could have an impact on their content generation plans. 
Question 6: Which YouTube category has the highest ratio of likes to dislikes on average?
Knowledge Used: Calculations and SQL queries are used in this question to find the typical like-to-dislike ratio for each YouTube category. To determine the category with the greatest average ratio, you would need to obtain information from the "YTVIDEO" table and conduct mathematical computations.
Importance/Usefulness: Knowing which categories have the highest ratios can provide competitive insights. Content creators can use this information to understand which categories tend to receive more positive engagement relative to negative feedback. This can help them decide which content areas to focus on or explore. By choosing categories with a larger ratio of likes to dislikes, marketers and advertisers can more effectively target their efforts. Better advertising outcomes and ROI may result from this.
Question 7: What is the average video length that a person watches on youtube?
Knowledge Used: It would be necessary to have access to user-level viewing data and the capacity to conduct data analysis in order to determine the typical length of a YouTube video that a user watches. In order to conduct this analysis, it would be necessary to calculate each user's average video viewing time, then add those results together to obtain the general average.
Importance/Usefulness: Planning and producing content can be guided by knowing the typical length of a video. It may have an impact on choices for the structure and format of videos. Individual users may be able to better organise their time on the site with the aid of this information. On the basis of desired video lengths, it can also be utilised to tailor their video recommendations.
Question 8: Which countries/regions contribute the most subscribers for a given channel?
Knowledge Used: You would require access to subscriber data with related nations or regions to ascertain which countries or regions contribute the most subscribers for a certain channel. Data aggregation and querying methods as well as an understanding of SQL or other data analysis tools would be necessary for this investigation.
Importance/Usefulness: This information can be used by content producers to target their advertising campaigns. They can concentrate on marketing and engagement plans aimed at the areas with the greatest contributions from subscribers. Knowing how subscribers are distributed geographically will help you better understand who is watching the channel. The preferences and interests of users from various locations can be better catered to by creators by modifying their material.
Question 9: What percentage of videos in the "Music" category are monetized with ads, and how does this compare to other categories?
Knowledge Used: Data aggregation, filtering, and percentage calculations are required to determine the proportion of videos in the "Music" category that are supported by advertisements. To determine the number of monetized videos in the "Music" category and to compare it to the overall number of videos in that category, you would need to perform a database query. Understanding SQL or data analysis software is necessary for this.
Importance/Usefulness: These details can be used by music channels and artists to comprehend the monetization environment in their field. They can use it to decide on content generation and monetization plans. Advertisers who are interested in the "Music" category can learn more about the ad space that is available and the rivalry for viewers' attention there.
Question 10: What is the correlation between the number of subscribers a channel has and the number of views its videos receive on average?
Knowledge Used: Knowing statistical analysis, specifically computing the correlation coefficient (e.g., Pearson correlation) between two variables, is necessary to determine the correlation between a channel's average number of views and subscribers. Access to subscriber and video view information for different channels is required.
Importance/Usefulness: This data can be used by content producers to determine how well their subscription base translates into video views. This knowledge can direct audience engagement initiatives and content strategies. Based on the correlation, content producers might modify their content strategy. If there is a large positive link, for instance, they might concentrate on subscriber growth to boost viewership.
Teamwork Description: 
Yug Vasani: Came up with ideas and formulated questions
Kevin Patel: Came up with ideas and formulated questions
Nisarg Patel: Came up with ideas and formulated questions
The team conducted a brainstorming session where each member contributes their ideas for these questions. We evaluated the questions to ensured that they align with the purpose and are actionable. Also, we discussed the relevance and feasibility of each question. We leveraged our collective knowledge from the course to formulate questions that would provide valuable insights and make effective use of the data.
