---
description: Paginated list of audience segments.
layout: schema
name: Audience List Response
properties_list:
- description: Array of audience segment objects.
  name: audiences
  type: array
- description: Total number of audience segments available.
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
schema_file: json-schema/retail-media-api-audience-list-response-schema.json
slug: retail-media-api-audience-list-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/albertsons/refs/heads/main/json-schema/retail-media-api-audience-list-response-schema.json\",\n  \"title\": \"Audience List Response\",\n  \"description\": \"Paginated list of audience segments.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"audiences\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Audience\"\n      },\n      \"description\": \"Array of audience segment objects.\"\n    },\n    \"total\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of audience segments available.\",\n      \"example\": 150\n    },\n    \"limit\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of results returned.\",\n      \"example\": 20\n    },\n    \"offset\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of results skipped.\",\n    \
  \  \"example\": 0\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/albertsons/refs/heads/main/json-schema/retail-media-api-audience-list-response-schema.json
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
title: Audience List Response
---
