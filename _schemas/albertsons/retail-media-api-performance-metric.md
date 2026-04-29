---
description: Performance metrics for an advertising campaign at a given time period.
layout: schema
name: Performance Metric
properties_list:
- description: Date of the metric data point.
  name: date
  type: string
- description: Campaign identifier associated with these metrics.
  name: campaignId
  type: string
- description: Number of ad impressions served.
  name: impressions
  type: integer
- description: Number of ad clicks recorded.
  name: clicks
  type: integer
- description: Number of conversions attributed to the campaign.
  name: conversions
  type: integer
- description: Total ad spend in USD for the period.
  name: spend
  type: number
- description: Return on ad spend ratio.
  name: roas
  type: number
- description: Click-through rate as a decimal (clicks / impressions).
  name: clickThroughRate
  type: number
provider_name: albertsons
provider_slug: albertsons
schema_file: json-schema/retail-media-api-performance-metric-schema.json
slug: retail-media-api-performance-metric
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/albertsons/refs/heads/main/json-schema/retail-media-api-performance-metric-schema.json\",\n  \"title\": \"Performance Metric\",\n  \"description\": \"Performance metrics for an advertising campaign at a given time period.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date of the metric data point.\",\n      \"example\": \"2026-03-15\"\n    },\n    \"campaignId\": {\n      \"type\": \"string\",\n      \"description\": \"Campaign identifier associated with these metrics.\",\n      \"example\": \"500123\"\n    },\n    \"impressions\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of ad impressions served.\",\n      \"example\": 45000\n    },\n    \"clicks\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of ad\
  \ clicks recorded.\",\n      \"example\": 675\n    },\n    \"conversions\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of conversions attributed to the campaign.\",\n      \"example\": 34\n    },\n    \"spend\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Total ad spend in USD for the period.\",\n      \"example\": 1250.0\n    },\n    \"roas\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Return on ad spend ratio.\",\n      \"example\": 4.2\n    },\n    \"clickThroughRate\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Click-through rate as a decimal (clicks / impressions).\",\n      \"example\": 0.015\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/albertsons/refs/heads/main/json-schema/retail-media-api-performance-metric-schema.json
tags:
- Grocery
- Retail
- Retail Media
- Advertising
- Campaigns
- Analytics
- Consumer Goods
- Food
- Pharmacy
title: Performance Metric
---
