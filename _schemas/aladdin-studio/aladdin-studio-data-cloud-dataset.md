---
description: An available dataset in the Aladdin Data Cloud
layout: schema
name: Dataset
properties_list:
- description: Unique dataset identifier (schema.table)
  name: datasetId
  type: string
- description: Dataset display name
  name: name
  type: string
- description: Snowflake schema
  name: schema
  type: string
- description: Dataset description
  name: description
  type: string
- description: Last update timestamp
  name: lastUpdated
  type: string
provider_name: Aladdin Studio
provider_slug: aladdin-studio
schema_file: json-schema/aladdin-studio-data-cloud-dataset-schema.json
slug: aladdin-studio-data-cloud-dataset
source_filename: aladdin-studio-data-cloud-dataset-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aladdin-studio/refs/heads/main/json-schema/aladdin-studio-data-cloud-dataset-schema.json\",\n  \"title\": \"Dataset\",\n  \"description\": \"An available dataset in the Aladdin Data Cloud\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"datasetId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique dataset identifier (schema.table)\",\n      \"example\": \"PORTFOLIO.HOLDINGS\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Dataset display name\",\n      \"example\": \"Portfolio Holdings\"\n    },\n    \"schema\": {\n      \"type\": \"string\",\n      \"description\": \"Snowflake schema\",\n      \"example\": \"PORTFOLIO\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Dataset description\",\n      \"example\": \"Daily portfolio positions and holdings\"\n\
  \    },\n    \"lastUpdated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Last update timestamp\",\n      \"example\": \"2026-04-19T00:00:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aladdin-studio/refs/heads/main/json-schema/aladdin-studio-data-cloud-dataset-schema.json
tags:
- Financial
- Investment Management
- Portfolio Analytics
- Risk Management
- Asset Management
- BlackRock
- Data Cloud
title: Dataset
---
