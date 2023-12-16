# Youtube_Consumer_Usage_Analysis
CNIT 372 Project Fall 2023

Group #7 Member: Kevin Patel, Nisarg Patel, and Yug Vasani.


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

The team engaged in a collaborative brainstorming session, during which each member actively contributed ideas for the specified questions. We assessed the questions to ensure their alignment with the intended purpose and feasibility for implementation. Additionally, we deliberated on the relevance and practicality of each question, drawing upon our collective knowledge from the course. Through this collaborative effort, we formulated a set of questions aimed at gaining valuable insights and optimizing data utilization. As a team, we collectively finalized a set of 10 questions, with each member contributing a minimum of 3 questions. Our collaborative efforts extended to crafting the queries, with Nisarg and Yug assisting in packaging them, and Kevin executing these packages in SQL. We convened as a team and collaborated on Google Slides, collectively working on the creation of the presentation. To ensure an equitable distribution of responsibilities, we divided the presentation tasks equally among all team members.
