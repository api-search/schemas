---
description: ''
layout: schema
name: NodeType
properties_list:
- description: Unique identifier for the node type
  name: node_type_id
  type: string
- description: Memory in megabytes
  name: memory_mb
  type: integer
- description: Number of CPU cores
  name: num_cores
  type: number
- description: Human-readable description
  name: description
  type: string
- description: Azure instance type identifier
  name: instance_type_id
  type: string
- description: Whether the node type is deprecated
  name: is_deprecated
  type: boolean
- description: Number of GPUs available
  name: num_gpus
  type: integer
- description: Category of the node type (General Purpose, Memory Optimized, etc.)
  name: category
  type: string
provider_name: Azure Databricks
provider_slug: azure-databricks
schema_file: json-schema/azure-databricks-node-type-schema.json
slug: azure-databricks-node-type
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"NodeType\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"node_type_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the node type\"\n    },\n    \"memory_mb\": {\n      \"type\": \"integer\",\n      \"description\": \"Memory in megabytes\"\n    },\n    \"num_cores\": {\n      \"type\": \"number\",\n      \"description\": \"Number of CPU cores\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable description\"\n    },\n    \"instance_type_id\": {\n      \"type\": \"string\",\n      \"description\": \"Azure instance type identifier\"\n    },\n    \"is_deprecated\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the node type is deprecated\"\n    },\n    \"num_gpus\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of GPUs available\"\n    },\n    \"category\": {\n \
  \     \"type\": \"string\",\n      \"description\": \"Category of the node type (General Purpose, Memory Optimized, etc.)\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-databricks/refs/heads/main/json-schema/azure-databricks-node-type-schema.json
tags:
- Analytics
- Apache Spark
- Big Data
- Data Engineering
- Machine Learning
title: NodeType
---
