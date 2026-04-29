---
description: ''
layout: schema
name: JobCluster
properties_list:
- description: A unique key for the job cluster. Referenced by tasks using job_cluster_key.
  name: job_cluster_key
  type: string
provider_name: Databricks
provider_slug: databricks
schema_file: json-schema/databricks-job-cluster-schema.json
slug: databricks-job-cluster
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"JobCluster\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"job_cluster_key\": {\n      \"type\": \"string\",\n      \"description\": \"A unique key for the job cluster. Referenced by tasks using job_cluster_key.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/databricks/refs/heads/main/json-schema/databricks-job-cluster-schema.json
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
title: JobCluster
---
