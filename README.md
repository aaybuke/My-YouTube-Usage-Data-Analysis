# My-YouTube-Usage-Data-Analysis
Description
This is my project for the DSA210 Introduction to Data Science Course (Fall 2024-2025) at Sabancı University.
In this project, I will analyze my personal YouTube usage data to gain insights into my viewing habits, preferences, and engagement patterns. The analysis will include exploratory data analysis (EDA), visualizations, and potentially machine learning models to uncover trends and make predictions based on my behavior on the platform.

WEBSITE: https://aaybuke.github.io/aybw-prj/

#Analyzing YouTube Watch Patterns Across Years and Age

By extracting and organizing data such as genres, watch times, and years, I aimed to uncover insights about my evolving preferences and explore how my age influenced the type and amount of content I consumed.

This analysis allowed me to visualize trends in my YouTube habits, such as the genres I preferred at different stages of life and how my total watch time varied over the years.



YouTube is one of the platforms I use most frequently for entertainment, learning, and general exploration. By analyzing my personal data, I hope to achieve a deeper understanding of:

How much time I spend on the platform.
My peak activity times and days.
The types of content I consume and how my preferences evolve.
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

Analyze my viewing behavior across years as i grow older.
Identify peaks in activity during specific periods .
Content Preferences

Examine the types of content I watch the most.
Explore changes in preferences over time (e.g., increasing focus on educational videos).
Engagement Analysis

Study how frequently I interact with videos .
Compare engagement rates across different content types over year.

Data Collection and Cleaning:

I used my YouTube watch history data and liked videos as the primary datasets.
The raw data included video URLs, timestamps, and other metadata. From these, I extracted key details such as video IDs, names, genres, and watch times.
I cleaned and structured the data into a consistent format using Python and libraries such as pandas.
Data Preparation:

Extracted video IDs from URLs using regular expressions.
Merged datasets to include liked videos, video genres, and watch times.
Calculated my age for each year based on the watch timestamp, enabling an analysis of age-based viewing patterns.
Analysis and Visualization:

Grouped data by year and genre to calculate the total watch time for each.
Created visualizations to showcase trends, such as how specific genres gained or lost popularity over time.
Compared yearly total watch times to identify periods of increased or decreased YouTube consumption.


Findings

Shifts in Behavior:

Early Years (2019–2021): These were years of higher engagement, driven by diverse genres and frequent viewing. This period reflects more free time and experimental behavior with content.
Later Years (2022–2025): Watching patterns became more refined and purposeful, focusing on fewer genres with a stronger inclination towards productivity and learning.
Impact of Life Stages:

The data aligns with natural life transitions. Increased responsibilities and other priorities led to reduced screen time and a shift in the type of content consumed.
Genre Contribution:

Educational content became more dominant in later years, highlighting a preference for self-improvement and learning.
Entertainment genres like Music and Movies remained consistent but played a secondary role compared to Education in the later years.
Key Observations:

Watching time trends show that while YouTube remained a constant part of my life, its role shifted from casual entertainment to a tool for personal growth and targeted engagement.
The significant decline in watch time in 2022 suggests a pivotal change in habits, possibly influenced by external factors like workload or personal growth.
Annual Watching Time by Genre
The line graph showing annual watching time by genre reveals key trends in my YouTube consumption patterns:

Peak Engagement (2020–2021):

During this period, genres like Music,comedy and Education peaked significantly, indicating high levels of interest and engagement.
These years coincide with times when I likely had more flexibility to explore diverse content.
This years saw the highest watch time, possibly due to global events (e.g., lockdowns) that increased screen time and accessibility.
Decline and Refocus (2022–2023):

A noticeable drop in total watching time occurs after 2022, particularly for genres like Lifestyle and Movies. This suggests a shift in priorities or reduced time spent on YouTube.
However, Education and Music remain consistently strong genres, reflecting more purposeful consumption.
Maturity in Viewing Patterns (2024–2025):

By 2024, Education takes a dominant position, suggesting a more deliberate focus on productive content.
Other genres, such as Comedy and Music, maintain moderate levels, while Sports and Travel consistently show the least engagement throughout the years.
Clustering Analysis: Age vs. Watching Time
The scatter plot with K-means clustering demonstrates distinct clusters in my YouTube viewing behavior over the years:


Watching time gradually declines after peaking in early adulthood (21–23). This demonstrates a natural progression of shifting priorities as I age.

The heatmap provides a detailed breakdown of watching time across genres for different age clusters.

Genre Dominance:

Education and Music emerge as the most dominant genres, especially in later years (ages 23–24), with the highest intensity in the heatmap.
Comedy and Movies maintain steady engagement but show less growth over time.
Sports, Technology, and Travel remain consistently underrepresented, with minimal engagement across all years.

Shifts in Focus:

Early years (ages 19–21) show diverse viewing habits with notable engagement across genres like Movies, Lifestyle, and Music.
As I aged, there was a clear shift toward more educational and meaningful content, reflecting a more intentional and focused consumption pattern.

Overall Observations
General Trends:

The data demonstrates a significant evolution in my YouTube consumption habits. Early years were characterized by diverse and experimental viewing, while later years showed a refined focus on specific genres like Education.
Watching time peaked during ages 21–22 and steadily declined thereafter, indicating shifting life priorities.
Genre-Specific Insights:

The rise of educational content over time suggests a growing interest in personal development and learning.
Consistent engagement with music highlights its importance as a form of entertainment across all years.

Limitations

Data-Specific Limitations
Partial Data: Some activities, such as incognito mode views, are not logged.
API Constraints: Metadata gathering is limited by API quotas and potential unavailability for certain videos.
Personal Limitations
Time Constraints: The project timeline may limit the depth of analysis.
Learning Curve: As I am still learning, advanced techniques might not be fully implemented.
*Understanding whether changes were due to personal preferences or external factors (e.g., global events) required careful consideration.


Future Work


Advanced Models: Experiment with machine learning models to predict video engagement or recommend content.
Long-Term Tracking: Update the analysis with newer data to observe trends over time.
Sentiment Analysis: Explore the sentiment of my comments and liked videos.
Interactive Visualizations: Develop a web app or dashboard for a more user-friendly presentation of the insights.

