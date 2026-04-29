---
description: Paginated list of campaigns.
layout: schema
name: Campaign List Response
properties_list:
- description: Array of campaign objects.
  name: campaigns
  type: array
- description: Total number of campaigns matching the query.
  name: total
  type: integer
- description: Maximum number of results returned.
  name: limit
  type: integer
- description: Number of results skipped.
  name: offset
  type: integer
provider_name: albertsons
provider_slug: albertsons
schema_file: json-schema/retail-media-api-campaign-list-response-schema.json
slug: retail-media-api-campaign-list-response
source_filename: retail-media-api-campaign-list-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/albertsons/refs/heads/main/json-schema/retail-media-api-campaign-list-response-schema.json\",\n  \"title\": \"Campaign List Response\",\n  \"description\": \"Paginated list of campaigns.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"campaigns\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Campaign\"\n      },\n      \"description\": \"Array of campaign objects.\"\n    },\n    \"total\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of campaigns matching the query.\",\n      \"example\": 42\n    },\n    \"limit\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of results returned.\",\n      \"example\": 20\n    },\n    \"offset\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of results skipped.\",\n      \"example\": 0\n\
  \    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/albertsons/refs/heads/main/json-schema/retail-media-api-campaign-list-response-schema.json
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
title: Campaign List Response
---
