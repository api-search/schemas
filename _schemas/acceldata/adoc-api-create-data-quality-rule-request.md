---
description: Request body for creating a data quality rule
layout: schema
name: CreateDataQualityRuleRequest
properties_list:
- description: Rule name
  name: name
  type: string
- description: Type of data quality check
  name: type
  type: string
- description: Dataset identifier to apply the rule to
  name: datasetId
  type: string
- description: Column to monitor
  name: columnName
  type: string
- description: Alert threshold as percentage (0-100)
  name: threshold
  type: number
- description: Severity of alerts triggered by this rule
  name: severity
  type: string
provider_name: Acceldata
provider_slug: acceldata
schema_file: json-schema/adoc-api-create-data-quality-rule-request-schema.json
slug: adoc-api-create-data-quality-rule-request
source_filename: adoc-api-create-data-quality-rule-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://acceldata.io/schemas/create-data-quality-rule-request.json\",\n  \"title\": \"CreateDataQualityRuleRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for creating a data quality rule\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Rule name\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of data quality check\"\n    },\n    \"datasetId\": {\n      \"type\": \"string\",\n      \"description\": \"Dataset identifier to apply the rule to\"\n    },\n    \"columnName\": {\n      \"type\": \"string\",\n      \"description\": \"Column to monitor\"\n    },\n    \"threshold\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Alert threshold as percentage (0-100)\"\n    },\n    \"severity\": {\n      \"type\": \"string\",\n      \"description\": \"Severity\
  \ of alerts triggered by this rule\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"type\",\n    \"datasetId\",\n    \"columnName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acceldata/refs/heads/main/json-schema/adoc-api-create-data-quality-rule-request-schema.json
tags:
- AI Agents
- Data Management
- Data Observability
- Data Pipeline
- Data Quality
- Intelligence
- Observability
title: CreateDataQualityRuleRequest
---
