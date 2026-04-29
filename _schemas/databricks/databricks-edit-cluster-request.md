---
description: ''
layout: schema
name: EditClusterRequest
properties_list:
- description: The unique identifier of the cluster to edit.
  name: cluster_id
  type: string
- description: The new name for the cluster.
  name: cluster_name
  type: string
- description: The runtime version.
  name: spark_version
  type: string
- description: The node type for worker nodes.
  name: node_type_id
  type: string
- description: The node type for the Spark driver.
  name: driver_node_type_id
  type: string
- description: Number of worker nodes.
  name: num_workers
  type: integer
- description: ''
  name: spark_conf
  type: object
- description: ''
  name: custom_tags
  type: object
- description: ''
  name: spark_env_vars
  type: object
- description: ''
  name: autotermination_minutes
  type: integer
- description: ''
  name: enable_elastic_disk
  type: boolean
- description: ''
  name: instance_pool_id
  type: string
- description: ''
  name: policy_id
  type: string
- description: ''
  name: data_security_mode
  type: string
- description: ''
  name: single_user_name
  type: string
- description: ''
  name: runtime_engine
  type: string
provider_name: Databricks
provider_slug: databricks
schema_file: json-schema/databricks-edit-cluster-request-schema.json
slug: databricks-edit-cluster-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EditClusterRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cluster_id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the cluster to edit.\"\n    },\n    \"cluster_name\": {\n      \"type\": \"string\",\n      \"description\": \"The new name for the cluster.\"\n    },\n    \"spark_version\": {\n      \"type\": \"string\",\n      \"description\": \"The runtime version.\"\n    },\n    \"node_type_id\": {\n      \"type\": \"string\",\n      \"description\": \"The node type for worker nodes.\"\n    },\n    \"driver_node_type_id\": {\n      \"type\": \"string\",\n      \"description\": \"The node type for the Spark driver.\"\n    },\n    \"num_workers\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of worker nodes.\"\n    },\n    \"spark_conf\": {\n      \"type\": \"object\"\n    },\n    \"custom_tags\": {\n      \"type\": \"\
  object\"\n    },\n    \"spark_env_vars\": {\n      \"type\": \"object\"\n    },\n    \"autotermination_minutes\": {\n      \"type\": \"integer\"\n    },\n    \"enable_elastic_disk\": {\n      \"type\": \"boolean\"\n    },\n    \"instance_pool_id\": {\n      \"type\": \"string\"\n    },\n    \"policy_id\": {\n      \"type\": \"string\"\n    },\n    \"data_security_mode\": {\n      \"type\": \"string\"\n    },\n    \"single_user_name\": {\n      \"type\": \"string\"\n    },\n    \"runtime_engine\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/databricks/refs/heads/main/json-schema/databricks-edit-cluster-request-schema.json
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
title: EditClusterRequest
---
