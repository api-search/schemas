---
description: Response containing tabular query results from a KQL query execution.
layout: schema
name: QueryResults
properties_list:
- description: Array of result tables.
  name: tables
  type: array
- description: Error information for partial errors.
  name: error
  type: object
provider_name: Azure Log Analytics
provider_slug: azure-log-analytics
schema_file: json-schema/query-api-query-results-schema.json
slug: query-api-query-results
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-log-analytics/refs/heads/main/json-schema/query-api-query-results-schema.json\",\n  \"title\": \"QueryResults\",\n  \"description\": \"Response containing tabular query results from a KQL query execution.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tables\": {\n      \"type\": \"array\",\n      \"description\": \"Array of result tables.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"The name of the table.\",\n            \"example\": \"PrimaryResult\"\n          },\n          \"columns\": {\n            \"type\": \"array\",\n            \"description\": \"Schema of the result columns.\",\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"name\"\
  : {\n                  \"type\": \"string\",\n                  \"description\": \"The column name.\"\n                },\n                \"type\": {\n                  \"type\": \"string\",\n                  \"description\": \"The data type of the column.\",\n                  \"enum\": [\"bool\", \"datetime\", \"decimal\", \"dynamic\", \"guid\", \"int\", \"long\", \"real\", \"string\", \"timespan\"]\n                }\n              }\n            }\n          },\n          \"rows\": {\n            \"type\": \"array\",\n            \"description\": \"Array of row data matching the column schema.\",\n            \"items\": {\n              \"type\": \"array\",\n              \"items\": {}\n            }\n          }\n        }\n      }\n    },\n    \"error\": {\n      \"type\": \"object\",\n      \"description\": \"Error information for partial errors.\",\n      \"properties\": {\n        \"code\": {\n          \"type\": \"string\",\n          \"description\": \"Error code identifier.\"\
  \n        },\n        \"message\": {\n          \"type\": \"string\",\n          \"description\": \"Human-readable error message.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-log-analytics/refs/heads/main/json-schema/query-api-query-results-schema.json
tags:
- Analytics
- Azure
- Cloud
- Logging
- Monitoring
title: QueryResults
---
