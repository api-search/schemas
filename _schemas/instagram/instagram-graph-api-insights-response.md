---
description: InsightsResponse schema from Instagram Graph API
layout: schema
name: InsightsResponse
properties_list:
- description: ''
  name: data
  type: array
provider_name: Instagram
provider_slug: instagram
schema_file: json-schema/instagram-graph-api-insights-response-schema.json
slug: instagram-graph-api-insights-response
source_filename: instagram-graph-api-insights-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/instagram/refs/heads/main/json-schema/instagram-graph-api-insights-response-schema.json\",\n  \"title\": \"InsightsResponse\",\n  \"description\": \"InsightsResponse schema from Instagram Graph API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"example\": \"impressions\"\n          },\n          \"period\": {\n            \"type\": \"string\",\n            \"example\": \"day\"\n          },\n          \"values\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"value\": {\n                  \"type\": \"integer\",\n                  \"example\": 1500\n\
  \                },\n                \"end_time\": {\n                  \"type\": \"string\",\n                  \"format\": \"date-time\",\n                  \"example\": \"2026-04-17T07:00:00+0000\"\n                }\n              }\n            }\n          },\n          \"title\": {\n            \"type\": \"string\",\n            \"example\": \"Impressions\"\n          },\n          \"description\": {\n            \"type\": \"string\",\n            \"example\": \"Total number of times the media has been seen.\"\n          },\n          \"id\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/instagram/refs/heads/main/json-schema/instagram-graph-api-insights-response-schema.json
tags:
- Instagram
- Meta
- Photos
- Social Media
- Videos
- Content Publishing
title: InsightsResponse
---
