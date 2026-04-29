---
description: A data quality or pipeline monitoring alert
layout: schema
name: Alert
properties_list:
- description: Unique alert identifier
  name: id
  type: string
- description: Alert title
  name: title
  type: string
- description: Alert severity level
  name: severity
  type: string
- description: Current alert status
  name: status
  type: string
- description: Data quality rule that triggered this alert
  name: ruleId
  type: string
- description: Dataset associated with the alert
  name: datasetId
  type: string
- description: Dataset name
  name: datasetName
  type: string
- description: Actual metric value that triggered the alert
  name: metricValue
  type: number
- description: Threshold that was exceeded
  name: threshold
  type: number
- description: When the alert was triggered
  name: triggeredAt
  type: string
provider_name: Acceldata
provider_slug: acceldata
schema_file: json-schema/adoc-api-alert-schema.json
slug: adoc-api-alert
source_filename: adoc-api-alert-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://acceldata.io/schemas/alert.json\",\n  \"title\": \"Alert\",\n  \"type\": \"object\",\n  \"description\": \"A data quality or pipeline monitoring alert\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique alert identifier\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Alert title\"\n    },\n    \"severity\": {\n      \"type\": \"string\",\n      \"description\": \"Alert severity level\",\n      \"enum\": [\n        \"critical\",\n        \"high\",\n        \"medium\",\n        \"low\"\n      ]\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current alert status\",\n      \"enum\": [\n        \"open\",\n        \"resolved\",\n        \"acknowledged\"\n      ]\n    },\n    \"ruleId\": {\n      \"type\": \"string\",\n      \"description\": \"Data quality rule that triggered\
  \ this alert\"\n    },\n    \"datasetId\": {\n      \"type\": \"string\",\n      \"description\": \"Dataset associated with the alert\"\n    },\n    \"datasetName\": {\n      \"type\": \"string\",\n      \"description\": \"Dataset name\"\n    },\n    \"metricValue\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Actual metric value that triggered the alert\"\n    },\n    \"threshold\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Threshold that was exceeded\"\n    },\n    \"triggeredAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the alert was triggered\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acceldata/refs/heads/main/json-schema/adoc-api-alert-schema.json
tags:
- AI Agents
- Data Management
- Data Observability
- Data Pipeline
- Data Quality
- Intelligence
- Observability
title: Alert
---
