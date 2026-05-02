---
description: ''
layout: schema
name: ClusterEvent
properties_list:
- description: Cluster ID associated with the event
  name: cluster_id
  type: string
- description: Timestamp of the event in epoch milliseconds
  name: timestamp
  type: integer
- description: Type of event
  name: type
  type: string
- description: Event-specific details
  name: details
  type: object
provider_name: Azure Databricks
provider_slug: microsoft-azure-databricks
schema_file: json-schema/azure-databricks-cluster-event-schema.json
slug: azure-databricks-cluster-event
source_filename: azure-databricks-cluster-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ClusterEvent\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cluster_id\": {\n      \"type\": \"string\",\n      \"description\": \"Cluster ID associated with the event\"\n    },\n    \"timestamp\": {\n      \"type\": \"integer\",\n      \"description\": \"Timestamp of the event in epoch milliseconds\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of event\"\n    },\n    \"details\": {\n      \"type\": \"object\",\n      \"description\": \"Event-specific details\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-databricks/refs/heads/main/json-schema/azure-databricks-cluster-event-schema.json
tags:
- Analytics
- Apache Spark
- Big Data
- Data Engineering
- Machine Learning
title: ClusterEvent
---
