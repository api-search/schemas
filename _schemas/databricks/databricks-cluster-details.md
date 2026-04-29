---
description: ''
layout: schema
name: ClusterDetails
properties_list:
- description: The unique identifier of the cluster.
  name: cluster_id
  type: string
- description: The human-readable name of the cluster.
  name: cluster_name
  type: string
- description: The runtime version of the cluster.
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
- description: The current state of the cluster.
  name: state
  type: string
- description: A message about the state of the cluster.
  name: state_message
  type: string
- description: The time the cluster was started in epoch milliseconds.
  name: start_time
  type: integer
- description: The time the cluster was terminated in epoch milliseconds.
  name: terminated_time
  type: integer
- description: The time when the cluster driver last lost its state in epoch milliseconds.
  name: last_state_loss_time
  type: integer
- description: The time of the last user activity on the cluster.
  name: last_activity_time
  type: integer
- description: The time the cluster was last restarted.
  name: last_restarted_time
  type: integer
- description: The email of the user who created the cluster.
  name: creator_user_name
  type: string
- description: The source that created the cluster.
  name: cluster_source
  type: string
- description: Spark configuration key-value pairs.
  name: spark_conf
  type: object
- description: Tags applied to the cluster.
  name: custom_tags
  type: object
- description: ''
  name: spark_env_vars
  type: object
- description: Auto-termination idle timeout in minutes.
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
- description: Default tags applied by Databricks.
  name: default_tags
  type: object
- description: ''
  name: cluster_log_status
  type: object
- description: ''
  name: termination_reason
  type: object
- description: ''
  name: disk_spec
  type: object
- description: ''
  name: executors
  type: array
- description: Port on the driver for JDBC/ODBC connections.
  name: jdbc_port
  type: integer
- description: The canonical Spark context identifier.
  name: spark_context_id
  type: integer
provider_name: Databricks
provider_slug: databricks
schema_file: json-schema/databricks-cluster-details-schema.json
slug: databricks-cluster-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ClusterDetails\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cluster_id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the cluster.\"\n    },\n    \"cluster_name\": {\n      \"type\": \"string\",\n      \"description\": \"The human-readable name of the cluster.\"\n    },\n    \"spark_version\": {\n      \"type\": \"string\",\n      \"description\": \"The runtime version of the cluster.\"\n    },\n    \"node_type_id\": {\n      \"type\": \"string\",\n      \"description\": \"The node type for worker nodes.\"\n    },\n    \"driver_node_type_id\": {\n      \"type\": \"string\",\n      \"description\": \"The node type for the Spark driver.\"\n    },\n    \"num_workers\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of worker nodes.\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"The current state\
  \ of the cluster.\"\n    },\n    \"state_message\": {\n      \"type\": \"string\",\n      \"description\": \"A message about the state of the cluster.\"\n    },\n    \"start_time\": {\n      \"type\": \"integer\",\n      \"description\": \"The time the cluster was started in epoch milliseconds.\"\n    },\n    \"terminated_time\": {\n      \"type\": \"integer\",\n      \"description\": \"The time the cluster was terminated in epoch milliseconds.\"\n    },\n    \"last_state_loss_time\": {\n      \"type\": \"integer\",\n      \"description\": \"The time when the cluster driver last lost its state in epoch milliseconds.\"\n    },\n    \"last_activity_time\": {\n      \"type\": \"integer\",\n      \"description\": \"The time of the last user activity on the cluster.\"\n    },\n    \"last_restarted_time\": {\n      \"type\": \"integer\",\n      \"description\": \"The time the cluster was last restarted.\"\n    },\n    \"creator_user_name\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"The email of the user who created the cluster.\"\n    },\n    \"cluster_source\": {\n      \"type\": \"string\",\n      \"description\": \"The source that created the cluster.\"\n    },\n    \"spark_conf\": {\n      \"type\": \"object\",\n      \"description\": \"Spark configuration key-value pairs.\"\n    },\n    \"custom_tags\": {\n      \"type\": \"object\",\n      \"description\": \"Tags applied to the cluster.\"\n    },\n    \"spark_env_vars\": {\n      \"type\": \"object\"\n    },\n    \"autotermination_minutes\": {\n      \"type\": \"integer\",\n      \"description\": \"Auto-termination idle timeout in minutes.\"\n    },\n    \"enable_elastic_disk\": {\n      \"type\": \"boolean\"\n    },\n    \"instance_pool_id\": {\n      \"type\": \"string\"\n    },\n    \"policy_id\": {\n      \"type\": \"string\"\n    },\n    \"data_security_mode\": {\n      \"type\": \"string\"\n    },\n    \"single_user_name\": {\n      \"type\": \"string\"\n    },\n    \"runtime_engine\": {\n      \"\
  type\": \"string\"\n    },\n    \"default_tags\": {\n      \"type\": \"object\",\n      \"description\": \"Default tags applied by Databricks.\"\n    },\n    \"cluster_log_status\": {\n      \"type\": \"object\"\n    },\n    \"termination_reason\": {\n      \"type\": \"object\"\n    },\n    \"disk_spec\": {\n      \"type\": \"object\"\n    },\n    \"executors\": {\n      \"type\": \"array\"\n    },\n    \"jdbc_port\": {\n      \"type\": \"integer\",\n      \"description\": \"Port on the driver for JDBC/ODBC connections.\"\n    },\n    \"spark_context_id\": {\n      \"type\": \"integer\",\n      \"description\": \"The canonical Spark context identifier.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/databricks/refs/heads/main/json-schema/databricks-cluster-details-schema.json
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
title: ClusterDetails
---
