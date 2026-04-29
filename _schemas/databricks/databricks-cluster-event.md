---
description: ''
layout: schema
name: ClusterEvent
properties_list:
- description: ''
  name: cluster_id
  type: string
- description: ''
  name: timestamp
  type: integer
- description: ''
  name: type
  type: string
- description: ''
  name: details
  type: object
provider_name: Databricks
provider_slug: databricks
schema_file: json-schema/databricks-cluster-event-schema.json
slug: databricks-cluster-event
source_filename: databricks-cluster-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ClusterEvent\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cluster_id\": {\n      \"type\": \"string\"\n    },\n    \"timestamp\": {\n      \"type\": \"integer\"\n    },\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"details\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/databricks/refs/heads/main/json-schema/databricks-cluster-event-schema.json
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
title: ClusterEvent
---
