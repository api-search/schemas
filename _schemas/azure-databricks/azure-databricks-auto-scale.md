---
description: ''
layout: schema
name: AutoScale
properties_list:
- description: Minimum number of workers
  name: min_workers
  type: integer
- description: Maximum number of workers
  name: max_workers
  type: integer
provider_name: Azure Databricks
provider_slug: azure-databricks
schema_file: json-schema/azure-databricks-auto-scale-schema.json
slug: azure-databricks-auto-scale
source_filename: azure-databricks-auto-scale-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AutoScale\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"min_workers\": {\n      \"type\": \"integer\",\n      \"description\": \"Minimum number of workers\"\n    },\n    \"max_workers\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of workers\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-databricks/refs/heads/main/json-schema/azure-databricks-auto-scale-schema.json
tags:
- Analytics
- Apache Spark
- Big Data
- Data Engineering
- Machine Learning
title: AutoScale
---
