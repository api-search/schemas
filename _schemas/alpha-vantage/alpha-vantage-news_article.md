---
description: News article with sentiment analysis scores
layout: schema
name: NewsArticle
properties_list:
- description: Article headline
  name: title
  type: string
- description: Article URL
  name: url
  type: string
- description: Publication timestamp in YYYYMMDDTHHMMSS format
  name: timePublished
  type: string
- description: Sentiment score from -1 (bearish) to +1 (bullish)
  name: overallSentimentScore
  type: number
- description: Human-readable sentiment label
  name: overallSentimentLabel
  type: string
provider_name: Alpha Vantage
provider_slug: alpha-vantage
schema_file: json-schema/alpha-vantage-news_article-schema.json
slug: alpha-vantage-news_article
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://www.alphavantage.co/schemas/alpha-vantage-news_article-schema.json\",\n  \"title\": \"NewsArticle\",\n  \"type\": \"object\",\n  \"description\": \"News article with sentiment analysis scores\",\n  \"properties\": {\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Article headline\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Article URL\"\n    },\n    \"timePublished\": {\n      \"type\": \"string\",\n      \"description\": \"Publication timestamp in YYYYMMDDTHHMMSS format\"\n    },\n    \"overallSentimentScore\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Sentiment score from -1 (bearish) to +1 (bullish)\"\n    },\n    \"overallSentimentLabel\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable sentiment label\",\n      \"enum\": [\n\
  \        \"Bearish\",\n        \"Somewhat-Bearish\",\n        \"Neutral\",\n        \"Somewhat-Bullish\",\n        \"Bullish\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alpha-vantage/refs/heads/main/json-schema/alpha-vantage-news_article-schema.json
tags:
- Financial
- Market Data
- Stocks
- Technical Indicators
- Economic Data
- Sentiment Analysis
title: NewsArticle
---
