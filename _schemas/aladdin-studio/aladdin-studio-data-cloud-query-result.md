---
description: Results from an Aladdin Data Cloud query execution
layout: schema
name: QueryResult
properties_list:
- description: Unique query execution identifier
  name: queryId
  type: string
- description: Query execution status
  name: status
  type: string
- description: Number of rows returned
  name: rowCount
  type: integer
- description: Column definitions
  name: columns
  type: array
- description: Result rows as arrays
  name: rows
  type: array
provider_name: Aladdin Studio
provider_slug: aladdin-studio
schema_file: json-schema/aladdin-studio-data-cloud-query-result-schema.json
slug: aladdin-studio-data-cloud-query-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aladdin-studio/refs/heads/main/json-schema/aladdin-studio-data-cloud-query-result-schema.json\",\n  \"title\": \"QueryResult\",\n  \"description\": \"Results from an Aladdin Data Cloud query execution\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"queryId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique query execution identifier\",\n      \"example\": \"qry-a1b2c3d4\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Query execution status\",\n      \"enum\": [\n        \"completed\",\n        \"running\",\n        \"failed\"\n      ],\n      \"example\": \"completed\"\n    },\n    \"rowCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of rows returned\",\n      \"example\": 100\n    },\n    \"columns\": {\n      \"type\": \"array\",\n      \"description\": \"Column\
  \ definitions\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"example\": \"PORTFOLIO_ID\"\n          },\n          \"type\": {\n            \"type\": \"string\",\n            \"example\": \"VARCHAR\"\n          }\n        }\n      }\n    },\n    \"rows\": {\n      \"type\": \"array\",\n      \"description\": \"Result rows as arrays\",\n      \"items\": {\n        \"type\": \"array\",\n        \"items\": {}\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aladdin-studio/refs/heads/main/json-schema/aladdin-studio-data-cloud-query-result-schema.json
tags:
- Financial
- Investment Management
- Portfolio Analytics
- Risk Management
- Asset Management
- BlackRock
- Data Cloud
title: QueryResult
---
