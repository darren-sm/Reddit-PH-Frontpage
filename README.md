# Reddit Front Page Web Scraping and Data Visualization

This project is divided into two parts: Web Scraping and Data Visualization. It would first gather the popular posts in reddit front page for Philippine users. The data will then be stored in a JSON flat file which will be visualized in the other Jupyter Notebook file.

### Web Scraping

Web scraping is also divided into two parts. The first part's purpose is to list out the popular posts in Philippines. What we'll get here are the links for the post.  Unfortunately, there is no API for this yet. So what I did is to send requests with proxy rotation to exceed the set limitations of bot requests.

![scraping.png](https://raw.githubusercontent.com/darren-sm/Reddit-PH-Frontpage/main/docs/scraping.png)

$^\text{Images from proxycrawl.com and secure.cerm.be}$

Multi-threading compensates to the reduced speed brought by proxy rotation. However, there's also a limit on how much requests we can send per minute or second to Reddit using their API. But `send_request` method has error handling in case we passed over the limits

### Data Visualization

This portion contains charts that summarize the data from Reddit front page. These charts are used to visually represent the data and make it easier to understand. Below are some examples of charts made from summarized 500 posts in Reddit front page with geo location set to `PH`

1. Word Cloud

   > most frequently occurring words (without English [Stop Words]([Stop word - Wikipedia](https://en.wikipedia.org/wiki/Stop_word))) 

   <img src="https://raw.githubusercontent.com/darren-sm/Reddit-PH-Frontpage/main/docs/wordcloud.png" alt="wordcloud.png (515×350) (raw.githubusercontent.com)" style="zoom:50%;" />

2. Popular Subreddits

   > Most frequent post subreddit in Reddit PH frontpage

   <img src="https://raw.githubusercontent.com/darren-sm/Reddit-PH-Frontpage/main/docs/subreddits.png" alt="subreddits.png (667×455) (raw.githubusercontent.com)" style="zoom:50%;" />

3. Post Categories

> Text posts = discussion. Videos can be hosted by reddit or linked (e.g. streamable). 

<img src="https://raw.githubusercontent.com/darren-sm/Reddit-PH-Frontpage/main/docs/category.png" alt="category.png (488×411) (raw.githubusercontent.com)" style="zoom:50%;" />

4. And more...

<img src="https://raw.githubusercontent.com/darren-sm/Reddit-PH-Frontpage/main/docs/emoji.png" alt="emoji.png (2560×1440) (raw.githubusercontent.com)" style="zoom:13%;" />



<img src="https://raw.githubusercontent.com/darren-sm/Reddit-PH-Frontpage/main/docs/nsfw.png" alt="nsfw.png (416×411) (raw.githubusercontent.com)" style="zoom:50%;" />

<img src="https://raw.githubusercontent.com/darren-sm/Reddit-PH-Frontpage/main/docs/upvote.png" alt="upvote.png (571×455) (raw.githubusercontent.com)" style="zoom:50%;" />