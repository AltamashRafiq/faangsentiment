# AWS Sentiment Analaysis Pipeline

This project implements an end to end serverless sentiment analysis pipeline using AWS Lambda for serverless deployment and AWS Comprehend to do the sentiment analysis. AWS Simple Queue Service (SQS) is used to queue messages stored in DynameDB for analaysis. The output is generated as JSON files packets, making them easy to use for further processing. The architecture of the pipeline is displayed below. Given the name of a FAANG company as a key value pair of the form {"name": "\<faang-company\>"}, the Wikipedia article for the named company is scraped and snippets of it are analyzed to determine their sentiment.
  
<p align="center">
  <img src="https://github.com/AltamashRafiq/faangsentiment/blob/main/img11.png" width="800">
</p>

# Sample Sentiments

**Message**: Instagram (commonly abbreviated to IG or Insta) is an American photo and video sharing social networking service created by Kevin Systrom and Mike Krieger.  
**Sentiment**: Neutral

**Message**: A face book or facebook is a common or web directory found at some American universities consisting of individuals’ photographs and names.'.  
**Sentiment**: Neutral
