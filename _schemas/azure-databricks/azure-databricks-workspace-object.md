---
description: ''
layout: schema
name: WorkspaceObject
properties_list:
- description: Type of the workspace object
  name: object_type
  type: string
- description: Absolute path of the object in the workspace
  name: path
  type: string
- description: Programming language of the object. Only applicable for notebooks.
  name: language
  type: string
- description: Unique identifier for the object
  name: object_id
  type: integer
- description: Creation timestamp in epoch milliseconds
  name: created_at
  type: integer
- description: Last modification timestamp in epoch milliseconds
  name: modified_at
  type: integer
- description: Resource ID for the object
  name: resource_id
  type: string
provider_name: Azure Databricks
provider_slug: azure-databricks
schema_file: json-schema/azure-databricks-workspace-object-schema.json
slug: azure-databricks-workspace-object
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"WorkspaceObject\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"object_type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of the workspace object\"\n    },\n    \"path\": {\n      \"type\": \"string\",\n      \"description\": \"Absolute path of the object in the workspace\"\n    },\n    \"language\": {\n      \"type\": \"string\",\n      \"description\": \"Programming language of the object. Only applicable for notebooks.\"\n    },\n    \"object_id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique identifier for the object\"\n    },\n    \"created_at\": {\n      \"type\": \"integer\",\n      \"description\": \"Creation timestamp in epoch milliseconds\"\n    },\n    \"modified_at\": {\n      \"type\": \"integer\",\n      \"description\": \"Last modification timestamp in epoch milliseconds\"\n    },\n    \"resource_id\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"Resource ID for the object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-databricks/refs/heads/main/json-schema/azure-databricks-workspace-object-schema.json
tags:
- Analytics
- Apache Spark
- Big Data
- Data Engineering
- Machine Learning
title: WorkspaceObject
---
