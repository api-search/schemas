---
description: Request body for executing a KQL query against a Log Analytics workspace.
layout: schema
name: QueryBody
properties_list:
- description: The KQL query to execute against the workspace.
  name: query
  type: string
- description: ISO 8601 duration or time interval for the query timespan.
  name: timespan
  type: string
- description: List of additional workspace IDs for cross-workspace queries.
  name: workspaces
  type: array
provider_name: Azure Log Analytics
provider_slug: azure-log-analytics
schema_file: json-schema/query-api-query-body-schema.json
slug: query-api-query-body
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-log-analytics/refs/heads/main/json-schema/query-api-query-body-schema.json\",\n  \"title\": \"QueryBody\",\n  \"description\": \"Request body for executing a KQL query against a Log Analytics workspace.\",\n  \"type\": \"object\",\n  \"required\": [\"query\"],\n  \"properties\": {\n    \"query\": {\n      \"type\": \"string\",\n      \"description\": \"The KQL query to execute against the workspace.\",\n      \"example\": \"AzureActivity | summarize count() by Category\"\n    },\n    \"timespan\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 8601 duration or time interval for the query timespan.\",\n      \"example\": \"P1D\"\n    },\n    \"workspaces\": {\n      \"type\": \"array\",\n      \"description\": \"List of additional workspace IDs for cross-workspace queries.\",\n      \"items\": {\n        \"type\": \"string\"\n\
  \      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-log-analytics/refs/heads/main/json-schema/query-api-query-body-schema.json
tags:
- Analytics
- Azure
- Cloud
- Logging
- Monitoring
title: QueryBody
---
