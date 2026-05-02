---
description: Represents a query request and response for the Azure Monitor Logs API and Application Insights query API, using Kusto Query Language (KQL).
layout: schema
name: Azure Monitor Log Query
properties_list:
- description: ''
  name: request
  type: object
- description: ''
  name: response
  type: object
provider_name: Azure Monitor
provider_slug: microsoft-azure-monitor
schema_file: json-schema/azure-monitor-log-query-schema.json
slug: azure-monitor-log-query
source_filename: azure-monitor-log-query-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schema.azure.com/monitor/log-query.json\",\n  \"title\": \"Azure Monitor Log Query\",\n  \"description\": \"Represents a query request and response for the Azure Monitor Logs API and Application Insights query API, using Kusto Query Language (KQL).\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"request\": {\n      \"$ref\": \"#/$defs/QueryBody\"\n    },\n    \"response\": {\n      \"$ref\": \"#/$defs/QueryResults\"\n    }\n  },\n  \"$defs\": {\n    \"QueryBody\": {\n      \"type\": \"object\",\n      \"required\": [\"query\"],\n      \"properties\": {\n        \"query\": {\n          \"type\": \"string\",\n          \"description\": \"The Analytics query in Kusto Query Language (KQL) format.\"\n        },\n        \"timespan\": {\n          \"type\": \"string\",\n          \"description\": \"The timespan over which to query data in ISO 8601 duration format (e.g., PT1H, P1D, P1DT12H).\"\
  \n        },\n        \"workspaces\": {\n          \"type\": \"array\",\n          \"items\": { \"type\": \"string\" },\n          \"description\": \"A list of workspace IDs to include in cross-workspace queries.\"\n        },\n        \"applications\": {\n          \"type\": \"array\",\n          \"items\": { \"type\": \"string\" },\n          \"description\": \"A list of Application Insights app IDs for cross-application queries.\"\n        }\n      }\n    },\n    \"QueryResults\": {\n      \"type\": \"object\",\n      \"required\": [\"tables\"],\n      \"properties\": {\n        \"tables\": {\n          \"type\": \"array\",\n          \"items\": { \"$ref\": \"#/$defs/Table\" },\n          \"description\": \"The list of tables, columns, and rows.\"\n        }\n      }\n    },\n    \"Table\": {\n      \"type\": \"object\",\n      \"required\": [\"name\", \"columns\", \"rows\"],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"\
  The name of the table.\"\n        },\n        \"columns\": {\n          \"type\": \"array\",\n          \"items\": { \"$ref\": \"#/$defs/Column\" },\n          \"description\": \"The list of columns in this table.\"\n        },\n        \"rows\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"array\",\n            \"items\": {}\n          },\n          \"description\": \"The resulting rows from this query. Each row is an array of values corresponding to the columns.\"\n        }\n      }\n    },\n    \"Column\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of this column.\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\"bool\", \"datetime\", \"dynamic\", \"int\", \"long\", \"real\", \"string\", \"guid\", \"decimal\", \"timespan\"],\n          \"description\": \"The data type of this column.\"\n        }\n\
  \      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-monitor/refs/heads/main/json-schema/azure-monitor-log-query-schema.json
tags:
- Application Insights
- Cloud
- Logs
- Metrics
- Monitoring
- Observability
title: Azure Monitor Log Query
---
