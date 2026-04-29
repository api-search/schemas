---
description: Pagination metadata for list responses.
layout: schema
name: Pagination Stats
properties_list:
- description: Number of records in this response.
  name: count
  type: integer
- description: Total number of records matching the query.
  name: total
  type: integer
provider_name: Agricultural Marketing Service
provider_slug: agricultural-marketing-service
schema_file: json-schema/mars-api-pagination-stats-schema.json
slug: mars-api-pagination-stats
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agricultural-marketing-service/refs/heads/main/json-schema/mars-api-pagination-stats-schema.json\",\n  \"title\": \"Pagination Stats\",\n  \"description\": \"Pagination metadata for list responses.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of records in this response.\",\n      \"example\": 100\n    },\n    \"total\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of records matching the query.\",\n      \"example\": 500\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agricultural-marketing-service/refs/heads/main/json-schema/mars-api-pagination-stats-schema.json
tags:
- Agriculture
- Federal Government
- Market News
- Livestock
- Dairy
- Fruits And Vegetables
- Cotton
- Tobacco
title: Pagination Stats
---
