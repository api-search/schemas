---
description: A data quality monitoring rule
layout: schema
name: DataQualityRule
properties_list:
- description: Unique rule identifier
  name: id
  type: string
- description: Rule name
  name: name
  type: string
- description: Type of data quality check
  name: type
  type: string
- description: Dataset the rule applies to
  name: datasetId
  type: string
- description: Dataset name
  name: datasetName
  type: string
- description: Column the rule monitors
  name: columnName
  type: string
- description: Alert threshold value (percentage or absolute)
  name: threshold
  type: number
- description: Alert severity when rule is violated
  name: severity
  type: string
- description: Rule activation status
  name: status
  type: string
- description: Rule creation timestamp
  name: createdAt
  type: string
provider_name: Acceldata
provider_slug: acceldata
schema_file: json-schema/adoc-api-data-quality-rule-schema.json
slug: adoc-api-data-quality-rule
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://acceldata.io/schemas/data-quality-rule.json\",\n  \"title\": \"DataQualityRule\",\n  \"type\": \"object\",\n  \"description\": \"A data quality monitoring rule\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique rule identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Rule name\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of data quality check\",\n      \"enum\": [\n        \"null_check\",\n        \"uniqueness_check\",\n        \"range_check\",\n        \"pattern_check\",\n        \"freshness_check\",\n        \"schema_check\",\n        \"custom\"\n      ]\n    },\n    \"datasetId\": {\n      \"type\": \"string\",\n      \"description\": \"Dataset the rule applies to\"\n    },\n    \"datasetName\": {\n      \"type\": \"string\",\n      \"description\": \"\
  Dataset name\"\n    },\n    \"columnName\": {\n      \"type\": \"string\",\n      \"description\": \"Column the rule monitors\"\n    },\n    \"threshold\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Alert threshold value (percentage or absolute)\"\n    },\n    \"severity\": {\n      \"type\": \"string\",\n      \"description\": \"Alert severity when rule is violated\",\n      \"enum\": [\n        \"critical\",\n        \"high\",\n        \"medium\",\n        \"low\"\n      ]\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Rule activation status\",\n      \"enum\": [\n        \"active\",\n        \"inactive\"\n      ]\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Rule creation timestamp\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acceldata/refs/heads/main/json-schema/adoc-api-data-quality-rule-schema.json
tags:
- AI Agents
- Data Management
- Data Observability
- Data Pipeline
- Data Quality
- Intelligence
- Observability
title: DataQualityRule
---
