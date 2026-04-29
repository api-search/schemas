---
description: Consumer segment definition
layout: schema
name: ConsumerSegment
properties_list:
- description: Unique segment identifier
  name: segment_id
  type: string
- description: Segment name
  name: name
  type: string
- description: Percentage of total market population
  name: size_pct
  type: number
- description: Average basket size in dollars
  name: avg_basket_size
  type: number
- description: Preferred shopping channels
  name: preferred_channels
  type: array
- description: Top categories for this segment
  name: key_categories
  type: array
provider_name: Circana
provider_slug: circana
schema_file: json-schema/liquid-data-consumer-segment-schema.json
slug: liquid-data-consumer-segment
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/circana/refs/heads/main/json-schema/liquid-data-consumer-segment-schema.json\",\n  \"title\": \"ConsumerSegment\",\n  \"description\": \"Consumer segment definition\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"segment_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique segment identifier\",\n      \"example\": \"seg-001\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Segment name\",\n      \"example\": \"Health-Conscious Shoppers\"\n    },\n    \"size_pct\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Percentage of total market population\",\n      \"example\": 18.5\n    },\n    \"avg_basket_size\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Average basket size in dollars\",\n      \"example\": 42.30\n\
  \    },\n    \"preferred_channels\": {\n      \"type\": \"array\",\n      \"description\": \"Preferred shopping channels\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"key_categories\": {\n      \"type\": \"array\",\n      \"description\": \"Top categories for this segment\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/circana/refs/heads/main/json-schema/liquid-data-consumer-segment-schema.json
tags:
- Analytics
- Consumer Data
- Market Research
- Retail
- CPG
- Point Of Sale
- Consumer Insights
- Business Intelligence
title: ConsumerSegment
---
