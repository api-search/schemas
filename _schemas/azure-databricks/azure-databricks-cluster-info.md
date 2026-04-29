---
description: ''
layout: schema
name: ClusterInfo
properties_list:
- description: Canonical identifier for the cluster
  name: cluster_id
  type: string
- description: Name of the cluster
  name: cluster_name
  type: string
- description: Databricks Runtime version
  name: spark_version
  type: string
- description: Node type for worker nodes
  name: node_type_id
  type: string
- description: Node type for the driver node
  name: driver_node_type_id
  type: string
- description: Number of worker nodes
  name: num_workers
  type: integer
- description: Current state of the cluster
  name: state
  type: string
- description: Message associated with the current state
  name: state_message
  type: string
- description: Username of the cluster creator
  name: creator_user_name
  type: string
- description: Time when the cluster was started (epoch milliseconds)
  name: start_time
  type: integer
- description: Time when the cluster was terminated (epoch milliseconds)
  name: terminated_time
  type: integer
- description: Time when the cluster driver lost its state (epoch milliseconds)
  name: last_state_loss_time
  type: integer
- description: Time when the cluster last had activity (epoch milliseconds)
  name: last_activity_time
  type: integer
- description: Automatically terminates the cluster after it is inactive for this time in minutes. 0 indicates no autotermination.
  name: autotermination_minutes
  type: integer
- description: Indicates the source that created the cluster
  name: cluster_source
  type: string
- description: Spark configuration key-value pairs
  name: spark_conf
  type: object
- description: ''
  name: custom_tags
  type: object
- description: ''
  name: init_scripts
  type: array
- description: ''
  name: spark_env_vars
  type: object
- description: ''
  name: enable_elastic_disk
  type: boolean
- description: ''
  name: instance_pool_id
  type: string
- description: ''
  name: policy_id
  type: string
- description: Tags applied automatically by Databricks
  name: default_tags
  type: object
- description: ''
  name: cluster_log_status
  type: object
- description: ''
  name: termination_reason
  type: object
- description: ''
  name: data_security_mode
  type: string
- description: ''
  name: single_user_name
  type: string
- description: ''
  name: runtime_engine
  type: string
- description: ''
  name: disk_spec
  type: object
- description: ''
  name: executors
  type: array
- description: Port on which the JDBC/ODBC server is listening
  name: jdbc_port
  type: integer
- description: Total memory in the cluster in megabytes
  name: cluster_memory_mb
  type: integer
- description: Total number of CPU cores in the cluster
  name: cluster_cores
  type: number
provider_name: Azure Databricks
provider_slug: azure-databricks
schema_file: json-schema/azure-databricks-cluster-info-schema.json
slug: azure-databricks-cluster-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ClusterInfo\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cluster_id\": {\n      \"type\": \"string\",\n      \"description\": \"Canonical identifier for the cluster\"\n    },\n    \"cluster_name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the cluster\"\n    },\n    \"spark_version\": {\n      \"type\": \"string\",\n      \"description\": \"Databricks Runtime version\"\n    },\n    \"node_type_id\": {\n      \"type\": \"string\",\n      \"description\": \"Node type for worker nodes\"\n    },\n    \"driver_node_type_id\": {\n      \"type\": \"string\",\n      \"description\": \"Node type for the driver node\"\n    },\n    \"num_workers\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of worker nodes\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"Current state of the cluster\"\n    },\n    \"state_message\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Message associated with the current state\"\n    },\n    \"creator_user_name\": {\n      \"type\": \"string\",\n      \"description\": \"Username of the cluster creator\"\n    },\n    \"start_time\": {\n      \"type\": \"integer\",\n      \"description\": \"Time when the cluster was started (epoch milliseconds)\"\n    },\n    \"terminated_time\": {\n      \"type\": \"integer\",\n      \"description\": \"Time when the cluster was terminated (epoch milliseconds)\"\n    },\n    \"last_state_loss_time\": {\n      \"type\": \"integer\",\n      \"description\": \"Time when the cluster driver lost its state (epoch milliseconds)\"\n    },\n    \"last_activity_time\": {\n      \"type\": \"integer\",\n      \"description\": \"Time when the cluster last had activity (epoch milliseconds)\"\n    },\n    \"autotermination_minutes\": {\n      \"type\": \"integer\",\n      \"description\": \"Automatically terminates the cluster after it is inactive\
  \ for this time in minutes. 0 indicates no autotermination.\"\n    },\n    \"cluster_source\": {\n      \"type\": \"string\",\n      \"description\": \"Indicates the source that created the cluster\"\n    },\n    \"spark_conf\": {\n      \"type\": \"object\",\n      \"description\": \"Spark configuration key-value pairs\"\n    },\n    \"custom_tags\": {\n      \"type\": \"object\"\n    },\n    \"init_scripts\": {\n      \"type\": \"array\"\n    },\n    \"spark_env_vars\": {\n      \"type\": \"object\"\n    },\n    \"enable_elastic_disk\": {\n      \"type\": \"boolean\"\n    },\n    \"instance_pool_id\": {\n      \"type\": \"string\"\n    },\n    \"policy_id\": {\n      \"type\": \"string\"\n    },\n    \"default_tags\": {\n      \"type\": \"object\",\n      \"description\": \"Tags applied automatically by Databricks\"\n    },\n    \"cluster_log_status\": {\n      \"type\": \"object\"\n    },\n    \"termination_reason\": {\n      \"type\": \"object\"\n    },\n    \"data_security_mode\"\
  : {\n      \"type\": \"string\"\n    },\n    \"single_user_name\": {\n      \"type\": \"string\"\n    },\n    \"runtime_engine\": {\n      \"type\": \"string\"\n    },\n    \"disk_spec\": {\n      \"type\": \"object\"\n    },\n    \"executors\": {\n      \"type\": \"array\"\n    },\n    \"jdbc_port\": {\n      \"type\": \"integer\",\n      \"description\": \"Port on which the JDBC/ODBC server is listening\"\n    },\n    \"cluster_memory_mb\": {\n      \"type\": \"integer\",\n      \"description\": \"Total memory in the cluster in megabytes\"\n    },\n    \"cluster_cores\": {\n      \"type\": \"number\",\n      \"description\": \"Total number of CPU cores in the cluster\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-databricks/refs/heads/main/json-schema/azure-databricks-cluster-info-schema.json
tags:
- Analytics
- Apache Spark
- Big Data
- Data Engineering
- Machine Learning
title: ClusterInfo
---
