---
description: Configuration for a cluster init script
layout: schema
name: InitScriptInfo
properties_list:
- description: ''
  name: workspace
  type: object
- description: ''
  name: volumes
  type: object
- description: ''
  name: dbfs
  type: object
- description: ''
  name: abfss
  type: object
provider_name: Azure Databricks
provider_slug: azure-databricks
schema_file: json-schema/azure-databricks-init-script-info-schema.json
slug: azure-databricks-init-script-info
source_filename: azure-databricks-init-script-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"InitScriptInfo\",\n  \"type\": \"object\",\n  \"description\": \"Configuration for a cluster init script\",\n  \"properties\": {\n    \"workspace\": {\n      \"type\": \"object\"\n    },\n    \"volumes\": {\n      \"type\": \"object\"\n    },\n    \"dbfs\": {\n      \"type\": \"object\"\n    },\n    \"abfss\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-databricks/refs/heads/main/json-schema/azure-databricks-init-script-info-schema.json
tags:
- Analytics
- Apache Spark
- Big Data
- Data Engineering
- Machine Learning
title: InitScriptInfo
---
