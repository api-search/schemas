---
description: ''
layout: schema
name: SparkNode
properties_list:
- description: ''
  name: private_ip
  type: string
- description: ''
  name: public_dns
  type: string
- description: ''
  name: node_id
  type: string
- description: ''
  name: instance_id
  type: string
- description: ''
  name: start_timestamp
  type: integer
- description: ''
  name: host_private_ip
  type: string
provider_name: Databricks
provider_slug: databricks
schema_file: json-schema/databricks-spark-node-schema.json
slug: databricks-spark-node
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SparkNode\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"private_ip\": {\n      \"type\": \"string\"\n    },\n    \"public_dns\": {\n      \"type\": \"string\"\n    },\n    \"node_id\": {\n      \"type\": \"string\"\n    },\n    \"instance_id\": {\n      \"type\": \"string\"\n    },\n    \"start_timestamp\": {\n      \"type\": \"integer\"\n    },\n    \"host_private_ip\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/databricks/refs/heads/main/json-schema/databricks-spark-node-schema.json
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
title: SparkNode
---
