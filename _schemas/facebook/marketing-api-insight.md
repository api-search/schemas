---
description: Advertising performance insight.
layout: schema
name: Insight
properties_list:
- description: Number of impressions.
  name: impressions
  type: string
- description: Number of clicks.
  name: clicks
  type: string
- description: Amount spent.
  name: spend
  type: string
- description: Cost per click.
  name: cpc
  type: string
- description: Cost per thousand impressions.
  name: cpm
  type: string
- description: Click-through rate.
  name: ctr
  type: string
- description: Number of unique users reached.
  name: reach
  type: string
- description: Start date of the insight period.
  name: date_start
  type: string
- description: End date of the insight period.
  name: date_stop
  type: string
provider_name: Facebook
provider_slug: facebook
schema_file: json-schema/marketing-api-insight-schema.json
slug: marketing-api-insight
source_filename: marketing-api-insight-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/facebook/refs/heads/main/json-schema/marketing-api-insight-schema.json\",\n  \"title\": \"Insight\",\n  \"description\": \"Advertising performance insight.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"impressions\": { \"type\": \"string\", \"description\": \"Number of impressions.\" },\n    \"clicks\": { \"type\": \"string\", \"description\": \"Number of clicks.\" },\n    \"spend\": { \"type\": \"string\", \"description\": \"Amount spent.\" },\n    \"cpc\": { \"type\": \"string\", \"description\": \"Cost per click.\" },\n    \"cpm\": { \"type\": \"string\", \"description\": \"Cost per thousand impressions.\" },\n    \"ctr\": { \"type\": \"string\", \"description\": \"Click-through rate.\" },\n    \"reach\": { \"type\": \"string\", \"description\": \"Number of unique users reached.\" },\n    \"date_start\": { \"type\": \"string\", \"format\"\
  : \"date\", \"description\": \"Start date of the insight period.\" },\n    \"date_stop\": { \"type\": \"string\", \"format\": \"date\", \"description\": \"End date of the insight period.\" }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/facebook/refs/heads/main/json-schema/marketing-api-insight-schema.json
tags:
- Advertising
- Content Publishing
- Messaging
- Social Media
- Social Networking
title: Insight
---
