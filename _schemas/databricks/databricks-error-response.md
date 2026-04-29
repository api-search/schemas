---
description: ''
layout: schema
name: ErrorResponse
properties_list:
- description: A machine-readable error code.
  name: error_code
  type: string
- description: A human-readable error message.
  name: message
  type: string
provider_name: Databricks
provider_slug: databricks
schema_file: json-schema/databricks-error-response-schema.json
slug: databricks-error-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ErrorResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"error_code\": {\n      \"type\": \"string\",\n      \"description\": \"A machine-readable error code.\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"A human-readable error message.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/databricks/refs/heads/main/json-schema/databricks-error-response-schema.json
tags:
- AI
- Analytics
- Apache Spark
- Big Data
- Clean Rooms
- Cloud Computing
- Data
- Data Analytics
- Data Engineering
- Data Governance
- Delta Lake
- Delta Sharing
- ETL
- Identity Management
- Lakehouse
- Machine Learning
- MLflow
- Model Serving
- Security
- SQL
- Unity Catalog
- Vector Search
- Visualize
title: ErrorResponse
---
