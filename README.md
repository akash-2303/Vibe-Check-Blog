# Vibe Check
## Unraveling Political Sentiment on YouTube

### Introduction:
In the digital age, social media platforms like YouTube have become significant arenas for political discussion. With millions of users sharing their opinions, these online conversations can offer valuable insights into public sentiment, media bias, and political leanings. Over the past semester, I dedicated my efforts to Project Vibe Check, a comprehensive initiative aimed at analyzing YouTube comments, particularly around election debates, to discern what people are saying, who they support, and how they perceive media portrayals of candidates.

### The First Phase: Collecting and Analyzing Preliminary Data
The most important component of any analysis, to nobody's surprise is data. Thus the first task was to collect youtube comments. This was chosen as these comments offered a treasure trove of real-time reactions and opinions from a diverse user base. We began by collecting comments from the 2020 U.S. election debate between Joe Biden and Donald Trump, using the [Youtube API](https://console.cloud.google.com/marketplace/product/google/youtube.googleapis.com), focusing on videos from the following channels CBS News, CSPAN, FOX News, NBC, Sky News. For those interested in the data, [you can access the 2020 election comments CSV files here.](https://github.com/akash-2303/Election-Data/tree/main/Debate_2020/data/datasets) There were a lot of attributes associated with each comment that could offer a lot of insights to those interested. Below is a sample of how the CSV structure looked like.

<p align="center"> <img src="Scrapped_example.png" alt="Sample of oyutube comments data" style="width: 80%;"> </p> <p align="center"><em>Source: CBS News 2020</em></p>   

After preprocessing the CSV files for all channels, I tried performing clustering with k=3 and tabulated the summary of my cluster interpretation after reverse encoding cluster centers. 

<p align="center"> <img src="2020_cluster summary.png" alt="Clustering summary 2020" style="width: 80%;"> </p> <p align="center"></p> 

This is up for interpretation. Next up was extending the same pipeline for first presidential debate of 2024 between Joe Biden and Donald Trump. This time, we gathered comments from MSNBC, C-SPAN, USA Today, NBC and Wall Street Journal. We recorded the results similarly([which you can check out here](https://github.com/akash-2303/Election-Data/tree/main/Debate_2024/data/datasets)) and I performed similar analysis. The results appeared more one sided this time. 


