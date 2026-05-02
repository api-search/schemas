---
description: ''
layout: schema
name: Error
properties_list:
- description: Databricks error code (e.g., RESOURCE_DOES_NOT_EXIST, INVALID_PARAMETER_VALUE)
  name: error_code
  type: string
- description: Human-readable error message
  name: message
  type: string
provider_name: Azure Databricks
provider_slug: microsoft-azure-databricks
schema_file: json-schema/azure-databricks-error-schema.json
slug: azure-databricks-error
source_filename: azure-databricks-error-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Error\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"error_code\": {\n      \"type\": \"string\",\n      \"description\": \"Databricks error code (e.g., RESOURCE_DOES_NOT_EXIST, INVALID_PARAMETER_VALUE)\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable error message\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-databricks/refs/heads/main/json-schema/azure-databricks-error-schema.json
tags:
- Analytics
- Apache Spark
- Big Data
- Data Engineering
- Machine Learning
title: Error
---
