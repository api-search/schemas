---
description: ''
layout: schema
name: SparkNode
properties_list:
- description: Private IP address of the node
  name: private_ip
  type: string
- description: Public DNS name of the node
  name: public_dns
  type: string
- description: Unique identifier for the node
  name: node_id
  type: string
- description: Azure instance identifier
  name: instance_id
  type: string
- description: Start time of the node (epoch milliseconds)
  name: start_timestamp
  type: integer
- description: Private IP address of the host
  name: host_private_ip
  type: string
provider_name: Azure Databricks
provider_slug: azure-databricks
schema_file: json-schema/azure-databricks-spark-node-schema.json
slug: azure-databricks-spark-node
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SparkNode\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"private_ip\": {\n      \"type\": \"string\",\n      \"description\": \"Private IP address of the node\"\n    },\n    \"public_dns\": {\n      \"type\": \"string\",\n      \"description\": \"Public DNS name of the node\"\n    },\n    \"node_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the node\"\n    },\n    \"instance_id\": {\n      \"type\": \"string\",\n      \"description\": \"Azure instance identifier\"\n    },\n    \"start_timestamp\": {\n      \"type\": \"integer\",\n      \"description\": \"Start time of the node (epoch milliseconds)\"\n    },\n    \"host_private_ip\": {\n      \"type\": \"string\",\n      \"description\": \"Private IP address of the host\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-databricks/refs/heads/main/json-schema/azure-databricks-spark-node-schema.json
tags:
- Analytics
- Apache Spark
- Big Data
- Data Engineering
- Machine Learning
title: SparkNode
---
