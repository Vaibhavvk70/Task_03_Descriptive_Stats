# Task_03_Descriptive_Stats
Task 03 Descriptive Statistics by Vaibhav Korde

# Social Media 2024 Election Analysis

This project analyzes social media content related to the 2024 US Presidential elections using:
- 🐍 Pure Python
- 🐼 Pandas
- 🧊 Polars

## 📊 Key Features

- Descriptive statistics (mean, std, count, min/max)
- JSON parsing for nested fields
- Performance comparison between Python, Pandas, and Polars

## 📈 Approach, Summary of findings, interesting insights and Lessons Learned for all 3 datasets

ADS DATASET

Pure Python: - Approach – Used csv, math and collections for basic operations. Used loops and Python functions in order to compute stats like mean, std, min, max, count and used counter for categorical summaries. Advantage of pure Python script is it doesn’t need any external libraries, and disadvantage is it is less efficient for large datasets and not ideal for scalability. 

Pandas: - Approach – Used read_csv, describe, nunique and value counts. The advantage of using Pandas is it is ideal for ad-hoc analysis and for moderate or large datasets. Cons of using this approach is Pandas requires more memory than Polars. 

Polars: - Approach – Used read_csv, describe, value_counts, group_by().agg() Pros of using Polars is it is highly memory efficient for large datasets and syntax is also quite like Pandas. Cons of using Polars is it is slightly on the harder side of the spectrum as compared to Pandas, so it is slightly difficult for beginners. 

According to me, Pandas is suitable for Junior Analysts, and it is easy to navigate and has more functionality than pure Python. 

Summary of findings – After cleaning the dataset (JSON structures), delivery_by_region column, it inferred that ads were heavily concentrated in states like Texas indicating targeted regional strategies. 

Interesting insights – Aggregated stats showed that some ads were low budget but highly engaging, while others had high spend but low visibility an indication of poor targeting or creative inefficiencies.

Lessons Learned – In Polars, there is no attribute called is_numeric like Pandas. 

FACEBOOK POSTS DATASET

Pure Python: - Approach – Defined functions to compute mean, standard deviation, min/max, used counter to get mode and unique counts and grouped data by Facebook_id and post_id using dictionaries. 

A similar approach to the previous Ads dataset was used for Pandas and Polars.

Summary of findings and interesting insights - Posts with images or videos typically showed higher Total Interactions, suggesting that visual media consistently drives more engagement. Mid-week (Tuesday to Thursday) posts saw the highest activity and engagement dropped significantly on weekends, suggesting timing affects reach and reactions. 

Lessons learned – Datetime conversion is crucial and necessary for accurate statistics and grouping of data. 

TWITTER POSTS DATASET

Pure Python: - Approach – Implemented logic for aggregating stats by source and id using dictionaries. 

Pandas: - Used .value_counts(). head(1) to extract the most frequent values.

Polars: - Applied .value_counts(). sort() with error handling and conditionals.

Summary of findings and interesting insights - Numeric columns like likes, views, retweets showed high standard deviation. The majority of posts had fewer than 500 likes, retweets, or replies, indicating that only a minority of tweets went viral. A few standout tweets amassed 10-20 times more interactions than the average and these are likely tied to hot political moments or prominent figures.

Lessons Learned – Removing null values heavy columns quoteId and inReplyToId simplified the analysis on the dataset.  

Instructions to run the code – I did the Python coding in Jupyter Notebook, so code can run and can be tested in Jupyter Notebook as well as in VS Code with Jupyter extension. 

## 🚀 Getting Started

```bash
# Clone the repo
git clone https://github.com/yourusername/social-media-election-analysis.git

# Open notebooks locally or in VS Code / Jupyter

