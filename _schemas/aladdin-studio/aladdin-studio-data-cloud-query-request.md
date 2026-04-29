---
description: SQL query request for the Aladdin Data Cloud
layout: schema
name: QueryRequest
properties_list:
- description: SQL query to execute against the Aladdin Data Cloud
  name: sql
  type: string
- description: Snowflake virtual warehouse to use
  name: warehouse
  type: string
- description: Query timeout in seconds
  name: timeout
  type: integer
- description: Maximum number of rows to return
  name: maxRows
  type: integer
provider_name: Aladdin Studio
provider_slug: aladdin-studio
schema_file: json-schema/aladdin-studio-data-cloud-query-request-schema.json
slug: aladdin-studio-data-cloud-query-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aladdin-studio/refs/heads/main/json-schema/aladdin-studio-data-cloud-query-request-schema.json\",\n  \"title\": \"QueryRequest\",\n  \"description\": \"SQL query request for the Aladdin Data Cloud\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sql\": {\n      \"type\": \"string\",\n      \"description\": \"SQL query to execute against the Aladdin Data Cloud\",\n      \"example\": \"SELECT * FROM PORTFOLIO_HOLDINGS WHERE AS_OF_DATE = CURRENT_DATE LIMIT 100\"\n    },\n    \"warehouse\": {\n      \"type\": \"string\",\n      \"description\": \"Snowflake virtual warehouse to use\",\n      \"example\": \"ANALYTICS_WH\"\n    },\n    \"timeout\": {\n      \"type\": \"integer\",\n      \"description\": \"Query timeout in seconds\",\n      \"example\": 300\n    },\n    \"maxRows\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum\
  \ number of rows to return\",\n      \"example\": 10000\n    }\n  },\n  \"required\": [\n    \"sql\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aladdin-studio/refs/heads/main/json-schema/aladdin-studio-data-cloud-query-request-schema.json
tags:
- Financial
- Investment Management
- Portfolio Analytics
- Risk Management
- Asset Management
- BlackRock
- Data Cloud
title: QueryRequest
---
