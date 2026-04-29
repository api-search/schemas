---
description: Paging from LinkedIn API
layout: schema
name: Paging
properties_list:
- description: Starting index
  name: start
  type: integer
- description: Number of results returned
  name: count
  type: integer
- description: Total number of results
  name: total
  type: integer
- description: ''
  name: links
  type: array
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-marketing-audience-insights-paging-schema.json
slug: linkedin-marketing-audience-insights-paging
source_filename: linkedin-marketing-audience-insights-paging-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-audience-insights-paging-schema.json\",\n  \"title\": \"Paging\",\n  \"description\": \"Paging from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"start\": {\n      \"type\": \"integer\",\n      \"description\": \"Starting index\",\n      \"example\": 0\n    },\n    \"count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of results returned\",\n      \"example\": 10\n    },\n    \"total\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of results\",\n      \"example\": 100\n    },\n    \"links\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/PagingLink\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-audience-insights-paging-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: Paging
---
