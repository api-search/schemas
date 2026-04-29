---
description: A registered dataset in Acceldata
layout: schema
name: Dataset
properties_list:
- description: Unique dataset identifier
  name: id
  type: string
- description: Dataset name (table or file name)
  name: name
  type: string
- description: Data source platform
  name: source
  type: string
- description: Database name
  name: database
  type: string
- description: Schema name
  name: schema
  type: string
- description: Overall data quality score (0-100)
  name: qualityScore
  type: number
- description: Last time the dataset was scanned
  name: lastScanned
  type: string
- description: Number of rows in the dataset
  name: rowCount
  type: integer
- description: Number of columns in the dataset
  name: columnCount
  type: integer
provider_name: Acceldata
provider_slug: acceldata
schema_file: json-schema/adoc-api-dataset-schema.json
slug: adoc-api-dataset
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://acceldata.io/schemas/dataset.json\",\n  \"title\": \"Dataset\",\n  \"type\": \"object\",\n  \"description\": \"A registered dataset in Acceldata\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique dataset identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Dataset name (table or file name)\"\n    },\n    \"source\": {\n      \"type\": \"string\",\n      \"description\": \"Data source platform\",\n      \"enum\": [\n        \"snowflake\",\n        \"databricks\",\n        \"bigquery\",\n        \"redshift\",\n        \"s3\",\n        \"hdfs\",\n        \"hive\",\n        \"postgres\"\n      ]\n    },\n    \"database\": {\n      \"type\": \"string\",\n      \"description\": \"Database name\"\n    },\n    \"schema\": {\n      \"type\": \"string\",\n      \"description\": \"Schema name\"\n    },\n   \
  \ \"qualityScore\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Overall data quality score (0-100)\"\n    },\n    \"lastScanned\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Last time the dataset was scanned\"\n    },\n    \"rowCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of rows in the dataset\"\n    },\n    \"columnCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of columns in the dataset\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acceldata/refs/heads/main/json-schema/adoc-api-dataset-schema.json
tags:
- AI Agents
- Data Management
- Data Observability
- Data Pipeline
- Data Quality
- Intelligence
- Observability
title: Dataset
---
