
# Topic Based Sentiment Analysis on Qatar World Cup Twitter Data

Qatar World Cup was full of surprises! From Saudi Arabia shocking the world by upsetting Argentina to Morocco's historic run to the semifinals, you must heard or witnessed those moments during that soccer craze. In this post, I will firt use **BERTopic** to **model topics** on tweets posted during the World Cup 2022. Then I will use **Hugging Face API** to do a **sentiment analysis** on those tweets. Finally, I will connect the topic modeling and sentiment analysis to conduct **topic based sentiment analysis**. 


## Visualization 
Figure 1: Topic Words for Top 10 Topics 
![](https://raw.githubusercontent.com/beeman-93/BERTopic-Qatar-World-Cup-Twitter-Data/main/result_1.png)

Figure 2: Topics over Time - Dynamic Topic Modeling
![](https://raw.githubusercontent.com/beeman-93/BERTopic-Qatar-World-Cup-Twitter-Data/main/result_2.png)

Figure 3: Word Cloud for Tweets with Positive Sentiments (sample size: 10,000)
![](https://raw.githubusercontent.com/beeman-93/BERTopic-Qatar-World-Cup-Twitter-Data/main/result_3.png)

Figure 4: Word Cloud for Tweets with Negative Sentiments (sample size: 10,000; sensitive words removed)
![](https://raw.githubusercontent.com/beeman-93/BERTopic-Qatar-World-Cup-Twitter-Data/main/result_4.png)

Figure 5: Sentiment Distribution on All Tweets (sample size: 300)
![](https://raw.githubusercontent.com/beeman-93/BERTopic-Qatar-World-Cup-Twitter-Data/main/result_5.png)

Figure 6: Sentiment Distribution on Topics (sample size: 300)
![](https://raw.githubusercontent.com/beeman-93/BERTopic-Qatar-World-Cup-Twitter-Data/main/topic_based_sentiment_distribution.png)

## Conclusion
- Based on the insights obtained from Figure 1, it appears that while there were initial controversies surrounding Qatar hosting the World Cup, the prevalent use of keywords such as "qatar2022" and "best" suggest that there is widespread appreciation for the efforts that Qatar has made in preparing for the event. Additionally, it is evident that among the many stars who played in the World Cup, Twitter users frequently discussed PSG teammates Mbappe and Messi, as indicated by the prominent appearance of their names as keywords.  
- Figure 2 revealed that the topic "qatar2022" and "best" was highly frequent across time, suggesting a widespread appreciation for Qatar's efforts in hosting the event.
- After performing sentiment analysis using the Hugging Face API, we grouped the tweets based on their sentiments (positive and negative) and visualized the most frequent words that appeared in each sentiment category in Figures 3 and 4. These visualizations highlighted the prevalence of positive sentiments, with words such as "congrats", "Messi", and "winner" appearing frequently in positive tweets, indicating a general admiration for Leo Messi and appreciation for the tournament. Negative tweets also had mentions of "Messi", but with less frequency, and frequently used the word "rigged", indicating a level of dissatisfaction with the refereeing in the tournament.
- Figure 5 showed that 60% of the 10,000 analyzed tweets exhibited positive sentiments, suggesting that most people were happy about the Qatar World Cup. Finally, we connected topic modeling and sentiment analysis to calculate the average sentiment of tweets in each topic, which is shown in Figure 6. The majority of the sentiments for each topic were positive, with topic 1 (argentina_world_cup_messi) showing the most positive sentiment, indicating a high level of satisfaction with Argentina winning the tournament. These findings highlight the potential of BERTopic and sentiment analysis as powerful tools for generating insights from large volumes of text data.
## API Reference

#### Hugging Face API - Conduct sentiment analysis

```http
  https://huggingface.co/inference-api
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `hf_token`      | `string` | **Required**. Your API key |

#### Check my tutorial on how to use Hugging Face API: 
```http
https://medium.com/@cd_24/using-bertopic-to-analyze-qatar-world-cup-twitter-data-part-3-b220630fd894
```




## Scrapping Tweets

#### snscrape - Scrape contents from social networking services (SNS)

```http
https://github.com/JustAnotherArchivist/snscrape
```

#### Check my tutorial on how to use snscrape to scrape twitter data: 
```http
https://medium.com/@cd_24/using-bertopic-to-analyze-qatar-world-cup-twitter-data-a5956c4949f1
```
## Code
The codes programmed in this project are displayed in this repository. Feel free to check and use them. 
