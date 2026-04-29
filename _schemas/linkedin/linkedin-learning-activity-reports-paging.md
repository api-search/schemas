---
description: Paging from LinkedIn API
layout: schema
name: Paging
properties_list:
- description: Total number of results
  name: total
  type: integer
- description: Number of results in this response
  name: count
  type: integer
- description: Starting index
  name: start
  type: integer
- description: ''
  name: links
  type: array
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-learning-activity-reports-paging-schema.json
slug: linkedin-learning-activity-reports-paging
source_filename: linkedin-learning-activity-reports-paging-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-learning-activity-reports-paging-schema.json\",\n  \"title\": \"Paging\",\n  \"description\": \"Paging from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"total\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of results\",\n      \"example\": 1\n    },\n    \"count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of results in this response\",\n      \"example\": 1\n    },\n    \"start\": {\n      \"type\": \"integer\",\n      \"description\": \"Starting index\",\n      \"example\": 0\n    },\n    \"links\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/PagingLink\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-learning-activity-reports-paging-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: Paging
---
