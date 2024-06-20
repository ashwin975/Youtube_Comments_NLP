# Youtube_Comments_NLP

## Introduction:
The primary objective of this project is to scrape comments rom a youtube video and do some analysis. I was actually researching about perfumes obviously got dragged into it when i was mindlessly scrolling instagram and got hit by a perfume ad. Thereby magically landing into perfume reviews, through which I found this perfume review videos by Demi Rawling.

Youtube link — https://youtu.be/oJqc2tLMObg Its a video on Top 10 Tom Ford perfumes. Quite an old video though(4 years)

## Libraries Used:

- ✅ Selenium Library for Scraping comments and usernames with chrome driver
- ✅ NLTK Library for Text classification and Semantic keyword matching 

## 𝍖 Data Processing: 
- Have ran the chrome driver to be headless for faster response, but you could also try commenting it out and run the code. If you find anyother faster way to scrape please let me know in the comments. I had initially referenced the code by François St-Amant.

- List of perfumes mentioned in the video was taken as a second dataframe with Perplexity.ai, I have taken out this list manually but there are ways to do this by parsing the video with python but lets save that for another day. 

- We could also use semantic string matching using any best available sentence transformers from HuggingFace or we could use any of the available LLMs to do the same (but for production deployments, for large datasets sentence transformers would suit the best).

- Each comment has sometimes one or more perfumes mentioned, so score is calculated for both the perfumes. Thats why, “I own black orchid…" comment has Beau de jour next to it. As it comes up twice, one for Beau de jour and one for black orchid.


## 📊 Data Visualization: 
- To perform this sentiment analysis and keyword matching, i’ve built a simple dashboard with Tableau that lets us quickly filter through the perfumes and their sentiment scores.

[Tableau Dashboard Link](https://public.tableau.com/views/YoutubeSentimentAnalysis/YoutubeComments-NLPAnalysis?:language=en-GB&:sid=&:display_count=n&:origin=viz_share_link)

![alt text](https://github.com/ashwin975/Youtube_Comments_NLP/blob/main/Dashboard_snap.jpg)


