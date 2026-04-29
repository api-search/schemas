---
description: ''
layout: schema
name: Pagination
properties_list:
- description: The current page number.
  name: pageNumber
  type: integer
- description: The number of items per page.
  name: pageSize
  type: integer
- description: The total number of items available.
  name: totalAvailable
  type: integer
provider_name: Tableau
provider_slug: tableau
schema_file: json-schema/tableau-rest-pagination-schema.json
slug: tableau-rest-pagination
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Pagination\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"pageNumber\": {\n      \"type\": \"integer\",\n      \"description\": \"The current page number.\"\n    },\n    \"pageSize\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of items per page.\"\n    },\n    \"totalAvailable\": {\n      \"type\": \"integer\",\n      \"description\": \"The total number of items available.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tableau/refs/heads/main/json-schema/tableau-rest-pagination-schema.json
tags:
- Analytics
- Business Intelligence
- Dashboards
- Data Visualization
title: Pagination
---
