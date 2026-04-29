---
description: Configuration for delivering Spark logs to a destination
layout: schema
name: ClusterLogConf
properties_list:
- description: ''
  name: dbfs
  type: object
- description: ''
  name: s3
  type: object
provider_name: Azure Databricks
provider_slug: azure-databricks
schema_file: json-schema/azure-databricks-cluster-log-conf-schema.json
slug: azure-databricks-cluster-log-conf
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ClusterLogConf\",\n  \"type\": \"object\",\n  \"description\": \"Configuration for delivering Spark logs to a destination\",\n  \"properties\": {\n    \"dbfs\": {\n      \"type\": \"object\"\n    },\n    \"s3\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-databricks/refs/heads/main/json-schema/azure-databricks-cluster-log-conf-schema.json
tags:
- Analytics
- Apache Spark
- Big Data
- Data Engineering
- Machine Learning
title: ClusterLogConf
---
