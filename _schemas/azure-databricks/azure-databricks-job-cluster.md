---
description: ''
layout: schema
name: JobCluster
properties_list:
- description: Unique key identifying this cluster specification
  name: job_cluster_key
  type: string
provider_name: Azure Databricks
provider_slug: azure-databricks
schema_file: json-schema/azure-databricks-job-cluster-schema.json
slug: azure-databricks-job-cluster
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"JobCluster\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"job_cluster_key\": {\n      \"type\": \"string\",\n      \"description\": \"Unique key identifying this cluster specification\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-databricks/refs/heads/main/json-schema/azure-databricks-job-cluster-schema.json
tags:
- Analytics
- Apache Spark
- Big Data
- Data Engineering
- Machine Learning
title: JobCluster
---
