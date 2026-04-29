---
description: Autoscaling configuration. When set, num_workers is ignored and the cluster scales between min_workers and max_workers.
layout: schema
name: AutoScale
properties_list:
- description: The minimum number of workers the cluster can scale down to.
  name: min_workers
  type: integer
- description: The maximum number of workers the cluster can scale up to.
  name: max_workers
  type: integer
provider_name: Databricks
provider_slug: databricks
schema_file: json-schema/databricks-auto-scale-schema.json
slug: databricks-auto-scale
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AutoScale\",\n  \"type\": \"object\",\n  \"description\": \"Autoscaling configuration. When set, num_workers is ignored and the cluster scales between min_workers and max_workers.\",\n  \"properties\": {\n    \"min_workers\": {\n      \"type\": \"integer\",\n      \"description\": \"The minimum number of workers the cluster can scale down to.\"\n    },\n    \"max_workers\": {\n      \"type\": \"integer\",\n      \"description\": \"The maximum number of workers the cluster can scale up to.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/databricks/refs/heads/main/json-schema/databricks-auto-scale-schema.json
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
title: AutoScale
---
