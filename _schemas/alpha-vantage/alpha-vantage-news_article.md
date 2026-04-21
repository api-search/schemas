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
tags:
- Financial
- Market Data
- Stocks
- Technical Indicators
- Economic Data
- Sentiment Analysis
title: NewsArticle
---
