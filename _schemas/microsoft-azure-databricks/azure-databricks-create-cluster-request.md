---
description: ''
layout: schema
name: CreateClusterRequest
properties_list:
- description: Cluster name requested by the user. Does not have to be unique. If not specified at creation, the cluster name is an empty string.
  name: cluster_name
  type: string
- description: The runtime version of the cluster. You can retrieve a list of available runtime versions using the spark-versions endpoint.
  name: spark_version
  type: string
- description: The node type for the worker nodes. Refer to list-node-types for available node types.
  name: node_type_id
  type: string
- description: The node type for the driver node. If unset, the driver node type is set as the same value as node_type_id.
  name: driver_node_type_id
  type: string
- description: Number of worker nodes. For a fixed-size cluster, set this to the desired number of workers. For an autoscaling cluster, this field is ignored in favor of autoscale settings.
  name: num_workers
  type: integer
- description: Map of Spark configuration key-value pairs. These are passed directly to the Spark driver and executors.
  name: spark_conf
  type: object
- description: SSH public keys for accessing cluster nodes
  name: ssh_public_keys
  type: array
- description: Custom tags applied to cluster resources. Databricks adds default tags in addition to any custom tags you specify.
  name: custom_tags
  type: object
- description: Init scripts to run when the cluster starts
  name: init_scripts
  type: array
- description: Map of environment variable key-value pairs for the Spark process.
  name: spark_env_vars
  type: object
- description: If true, enable autoscaling local storage. When enabled, the amount of disk space used by the cluster auto-adjusts.
  name: enable_elastic_disk
  type: boolean
- description: ID of the instance pool to use for cluster nodes. If specified, the cluster uses the instance pool for both driver and worker nodes.
  name: instance_pool_id
  type: string
- description: Identifier of the cluster policy used to create the cluster.
  name: policy_id
  type: string
- description: Whether to enable local disk encryption for the cluster
  name: enable_local_disk_encryption
  type: boolean
- description: The runtime engine to use. PHOTON provides optimized query execution.
  name: runtime_engine
  type: string
- description: Data security mode for the cluster. Determines how data access is controlled.
  name: data_security_mode
  type: string
- description: The name of the single user who can execute commands on the cluster. Required when data_security_mode is SINGLE_USER.
  name: single_user_name
  type: string
provider_name: Azure Databricks
provider_slug: microsoft-azure-databricks
schema_file: json-schema/azure-databricks-create-cluster-request-schema.json
slug: azure-databricks-create-cluster-request
source_filename: azure-databricks-create-cluster-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateClusterRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cluster_name\": {\n      \"type\": \"string\",\n      \"description\": \"Cluster name requested by the user. Does not have to be unique. If not specified at creation, the cluster name is an empty string.\"\n    },\n    \"spark_version\": {\n      \"type\": \"string\",\n      \"description\": \"The runtime version of the cluster. You can retrieve a list of available runtime versions using the spark-versions endpoint.\"\n    },\n    \"node_type_id\": {\n      \"type\": \"string\",\n      \"description\": \"The node type for the worker nodes. Refer to list-node-types for available node types.\"\n    },\n    \"driver_node_type_id\": {\n      \"type\": \"string\",\n      \"description\": \"The node type for the driver node. If unset, the driver node type is set as the same value as node_type_id.\"\n    },\n    \"num_workers\"\
  : {\n      \"type\": \"integer\",\n      \"description\": \"Number of worker nodes. For a fixed-size cluster, set this to the desired number of workers. For an autoscaling cluster, this field is ignored in favor of autoscale settings.\"\n    },\n    \"spark_conf\": {\n      \"type\": \"object\",\n      \"description\": \"Map of Spark configuration key-value pairs. These are passed directly to the Spark driver and executors.\"\n    },\n    \"ssh_public_keys\": {\n      \"type\": \"array\",\n      \"description\": \"SSH public keys for accessing cluster nodes\"\n    },\n    \"custom_tags\": {\n      \"type\": \"object\",\n      \"description\": \"Custom tags applied to cluster resources. Databricks adds default tags in addition to any custom tags you specify.\"\n    },\n    \"init_scripts\": {\n      \"type\": \"array\",\n      \"description\": \"Init scripts to run when the cluster starts\"\n    },\n    \"spark_env_vars\": {\n      \"type\": \"object\",\n      \"description\": \"Map of\
  \ environment variable key-value pairs for the Spark process.\"\n    },\n    \"enable_elastic_disk\": {\n      \"type\": \"boolean\",\n      \"description\": \"If true, enable autoscaling local storage. When enabled, the amount of disk space used by the cluster auto-adjusts.\"\n    },\n    \"instance_pool_id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the instance pool to use for cluster nodes. If specified, the cluster uses the instance pool for both driver and worker nodes.\"\n    },\n    \"policy_id\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the cluster policy used to create the cluster.\"\n    },\n    \"enable_local_disk_encryption\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to enable local disk encryption for the cluster\"\n    },\n    \"runtime_engine\": {\n      \"type\": \"string\",\n      \"description\": \"The runtime engine to use. PHOTON provides optimized query execution.\"\n    },\n    \"data_security_mode\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Data security mode for the cluster. Determines how data access is controlled.\"\n    },\n    \"single_user_name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the single user who can execute commands on the cluster. Required when data_security_mode is SINGLE_USER.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-databricks/refs/heads/main/json-schema/azure-databricks-create-cluster-request-schema.json
tags:
- Analytics
- Apache Spark
- Big Data
- Data Engineering
- Machine Learning
title: CreateClusterRequest
---
