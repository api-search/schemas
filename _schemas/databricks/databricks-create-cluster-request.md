---
description: ''
layout: schema
name: CreateClusterRequest
properties_list:
- description: A human-readable name for the cluster. This does not need to be unique.
  name: cluster_name
  type: string
- description: The runtime version of the cluster. You can retrieve a list of available runtime versions using the Runtime Versions API.
  name: spark_version
  type: string
- description: The node type for worker nodes. This field determines the cloud provider instance type.
  name: node_type_id
  type: string
- description: The node type for the Spark driver. If not specified, defaults to the same value as node_type_id.
  name: driver_node_type_id
  type: string
- description: Number of worker nodes for a fixed-size cluster. A cluster has one Spark driver and num_workers executors. Set to 0 for a single-node cluster.
  name: num_workers
  type: integer
- description: A map of Spark configuration key-value pairs. These override the default Spark configuration values.
  name: spark_conf
  type: object
- description: Additional tags for cluster resources. Tags are propagated to the cloud provider for cost tracking.
  name: custom_tags
  type: object
- description: Environment variables for all Spark processes. Use {{secrets/scope/key}} to reference secrets.
  name: spark_env_vars
  type: object
- description: Minutes of inactivity after which the cluster is automatically terminated. 0 disables auto-termination.
  name: autotermination_minutes
  type: integer
- description: Whether to autoscale local storage. When enabled, Databricks monitors disk usage and attaches additional disks as needed.
  name: enable_elastic_disk
  type: boolean
- description: The optional ID of the instance pool to use for cluster nodes.
  name: instance_pool_id
  type: string
- description: The ID of the cluster policy to apply. Cluster policies constrain the configuration settings.
  name: policy_id
  type: string
- description: Whether to encrypt data on local disks.
  name: enable_local_disk_encryption
  type: boolean
- description: The runtime engine. PHOTON enables the Photon vectorized query engine for faster performance.
  name: runtime_engine
  type: string
- description: Data security mode for the cluster.
  name: data_security_mode
  type: string
- description: The user name (email) of the single user for SINGLE_USER access mode.
  name: single_user_name
  type: string
- description: Init scripts to run when the cluster starts.
  name: init_scripts
  type: array
- description: SSH public keys to add to each Spark node.
  name: ssh_public_keys
  type: array
provider_name: Databricks
provider_slug: databricks
schema_file: json-schema/databricks-create-cluster-request-schema.json
slug: databricks-create-cluster-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateClusterRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cluster_name\": {\n      \"type\": \"string\",\n      \"description\": \"A human-readable name for the cluster. This does not need to be unique.\"\n    },\n    \"spark_version\": {\n      \"type\": \"string\",\n      \"description\": \"The runtime version of the cluster. You can retrieve a list of available runtime versions using the Runtime Versions API.\"\n    },\n    \"node_type_id\": {\n      \"type\": \"string\",\n      \"description\": \"The node type for worker nodes. This field determines the cloud provider instance type.\"\n    },\n    \"driver_node_type_id\": {\n      \"type\": \"string\",\n      \"description\": \"The node type for the Spark driver. If not specified, defaults to the same value as node_type_id.\"\n    },\n    \"num_workers\": {\n      \"type\": \"integer\",\n      \"description\": \"Number\
  \ of worker nodes for a fixed-size cluster. A cluster has one Spark driver and num_workers executors. Set to 0 for a single-node cluster.\"\n    },\n    \"spark_conf\": {\n      \"type\": \"object\",\n      \"description\": \"A map of Spark configuration key-value pairs. These override the default Spark configuration values.\"\n    },\n    \"custom_tags\": {\n      \"type\": \"object\",\n      \"description\": \"Additional tags for cluster resources. Tags are propagated to the cloud provider for cost tracking.\"\n    },\n    \"spark_env_vars\": {\n      \"type\": \"object\",\n      \"description\": \"Environment variables for all Spark processes. Use {{secrets/scope/key}} to reference secrets.\"\n    },\n    \"autotermination_minutes\": {\n      \"type\": \"integer\",\n      \"description\": \"Minutes of inactivity after which the cluster is automatically terminated. 0 disables auto-termination.\"\n    },\n    \"enable_elastic_disk\": {\n      \"type\": \"boolean\",\n      \"description\"\
  : \"Whether to autoscale local storage. When enabled, Databricks monitors disk usage and attaches additional disks as needed.\"\n    },\n    \"instance_pool_id\": {\n      \"type\": \"string\",\n      \"description\": \"The optional ID of the instance pool to use for cluster nodes.\"\n    },\n    \"policy_id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the cluster policy to apply. Cluster policies constrain the configuration settings.\"\n    },\n    \"enable_local_disk_encryption\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to encrypt data on local disks.\"\n    },\n    \"runtime_engine\": {\n      \"type\": \"string\",\n      \"description\": \"The runtime engine. PHOTON enables the Photon vectorized query engine for faster performance.\"\n    },\n    \"data_security_mode\": {\n      \"type\": \"string\",\n      \"description\": \"Data security mode for the cluster.\"\n    },\n    \"single_user_name\": {\n      \"type\": \"string\",\n \
  \     \"description\": \"The user name (email) of the single user for SINGLE_USER access mode.\"\n    },\n    \"init_scripts\": {\n      \"type\": \"array\",\n      \"description\": \"Init scripts to run when the cluster starts.\"\n    },\n    \"ssh_public_keys\": {\n      \"type\": \"array\",\n      \"description\": \"SSH public keys to add to each Spark node.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/databricks/refs/heads/main/json-schema/databricks-create-cluster-request-schema.json
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
title: CreateClusterRequest
---
