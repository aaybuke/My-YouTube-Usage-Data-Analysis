# My-YouTube-Usage-Data-Analysis
Description
This is my project for the CS210 Introduction to Data Science Course (Fall 2023-2024) at Sabancı University.
In this project, I will analyze my personal YouTube usage data to gain insights into my viewing habits, preferences, and engagement patterns. The analysis will include exploratory data analysis (EDA), visualizations, and potentially machine learning models to uncover trends and make predictions based on my behavior on the platform.


Table of Contents

Motivation
Objectives
Tools
Data Source
Exported YouTube Data
Supplementary Data
Data Processing
Planned Visualizations
Planned Analyses
Temporal Patterns
Content Preferences
Engagement Analysis
Findings
Limitations
Data-Specific Limitations
Personal Limitations
Future Work


Motivation

YouTube is one of the platforms I use most frequently for entertainment, learning, and general exploration. By analyzing my personal data, I hope to achieve a deeper understanding of:

How much time I spend on the platform.
My peak activity times and days.
The types of content I consume and how my preferences evolve.
My engagement patterns, such as liking, commenting, or subscribing to channels.
This project is not only a way to learn about myself but also an opportunity to apply and showcase data science techniques on a real dataset that matters to me.

Objectives

To identify and analyze patterns in my YouTube viewing habits.
To explore the impact of time, content type, and other factors on my engagement.
To create meaningful visualizations that convey insights effectively.
Optionally, to use machine learning techniques to predict or classify aspects of my YouTube activity (e.g., predicting content categories or engagement levels).
Tools
The project will utilize the following tools and libraries:

Python: The primary programming language for analysis and visualization.
Jupyter Notebook: For documenting the project workflow.
Pandas: For data cleaning, manipulation, and analysis.
Numpy: For mathematical operations.
Matplotlib and Seaborn: For creating static visualizations.
Plotly: For interactive visualizations and dashboards.
Scikit-learn: For potential machine learning modeling.
YouTube Data API: For collecting additional metadata about videos and channels.


Data Source

Exported YouTube Data
I requested my YouTube usage data via Google Takeout, which includes:

Watch History: Video titles, watch timestamps, and channel names.
Search History: Queries made on YouTube, with timestamps.
Subscriptions: A list of channels I am subscribed to.
Likes and Comments: Logs of liked videos and comments made.
Supplementary Data
To enhance the analysis, I will collect metadata such as video categories, tags, view counts, and publication dates using the YouTube Data API. This data will provide context to the exported dataset, enabling more detailed insights.

Data Processing

The raw data contains redundant information and sensitive details. The preprocessing steps will include:

Cleaning: Removing unnecessary fields (e.g., IP addresses) and handling missing or inconsistent values.
Timestamp Conversion: Converting UTC timestamps to my local timezone and extracting useful features such as day of the week, time of day, and month.
Categorization: Categorizing videos based on their metadata (e.g., content type, tags).
Anonymization: Hiding any personal or sensitive information in the dataset.
Feature Engineering: Creating new columns like:
Session durations (grouping consecutive watch times).
Engagement levels (e.g., like/comment ratio).


Planned Visualizations


Bar Charts: To show the distribution of videos watched by content category and channel.
Histograms: To visualize activity patterns by time of day and day of the week.
Heatmaps: To identify correlations between watch time, video popularity, and engagement levels.
Scatter Plots: To explore relationships between video metrics (e.g., duration vs. views).
Interactive Dashboards: Allowing exploration of specific patterns dynamically.


Planned Analyses

Temporal Patterns

Analyze my viewing behavior across different days and times.
Identify peaks in activity during specific periods (e.g., holidays, weekends).
Content Preferences

Examine the types of content I watch the most.
Explore changes in preferences over time (e.g., increasing focus on educational videos).
Engagement Analysis

Study how frequently I interact with videos (e.g., likes, comments, or subscriptions).
Compare engagement rates across different content types or channels.


Findings

This section will summarize the key insights discovered during the project, such as:

Patterns in my activity over time.
Trends in content consumption.
Factors influencing my engagement with videos.

Limitations

Data-Specific Limitations
Partial Data: Some activities, such as incognito mode views, are not logged.
API Constraints: Metadata gathering is limited by API quotas and potential unavailability for certain videos.
Personal Limitations
Time Constraints: The project timeline may limit the depth of analysis.
Learning Curve: As I am still learning, advanced techniques might not be fully implemented.


Future Work


Advanced Models: Experiment with machine learning models to predict video engagement or recommend content.
Long-Term Tracking: Update the analysis with newer data to observe trends over time.
Sentiment Analysis: Explore the sentiment of my comments and liked videos.
Interactive Visualizations: Develop a web app or dashboard for a more user-friendly presentation of the insights.
