---
description: Schema representing a Databricks cluster, which is a managed cloud resource for running data engineering and data science workloads on Apache Spark. Clusters can be configured with fixed or autoscaling worker counts, various node types, and cloud-provider-specific attributes.
layout: schema
name: Databricks Cluster
properties_list:
- description: The unique identifier assigned to the cluster by Databricks. This ID is generated during cluster creation and is used to reference the cluster in all subsequent API calls.
  name: cluster_id
  type: string
- description: A human-readable name for the cluster. This does not need to be unique within the workspace.
  name: cluster_name
  type: string
- description: The Databricks Runtime version of the cluster, which determines the versions of Apache Spark, Scala, Java, Python, R, and installed libraries. Use the Runtime Versions API to retrieve available versio
  name: spark_version
  type: string
- description: The cloud provider instance type for worker nodes. Determines the compute and memory resources available to each worker.
  name: node_type_id
  type: string
- description: The cloud provider instance type for the Spark driver node. If not specified, defaults to the same value as node_type_id.
  name: driver_node_type_id
  type:
  - string
  - 'null'
- description: The number of worker nodes in a fixed-size cluster. A cluster has one Spark driver and num_workers executors. Set to 0 for a single-node cluster where the driver acts as both driver and worker.
  name: num_workers
  type: integer
- description: Autoscaling configuration. When set, num_workers is ignored and the cluster dynamically scales between min_workers and max_workers based on workload.
  name: autoscale
  type:
  - object
  - 'null'
- description: The current state of the cluster in its lifecycle.
  name: state
  type: string
- description: A human-readable message providing additional information about the current cluster state, such as the reason for termination.
  name: state_message
  type: string
- description: The time when the cluster was started, represented as epoch milliseconds (Unix timestamp in milliseconds).
  name: start_time
  type: integer
- description: The time when the cluster was terminated, represented as epoch milliseconds.
  name: terminated_time
  type: integer
- description: The time when the cluster driver last lost its state, represented as epoch milliseconds. This occurs when the driver node is lost or restarted.
  name: last_state_loss_time
  type: integer
- description: The time of the last user activity on the cluster, used for auto-termination calculations. Represented as epoch milliseconds.
  name: last_activity_time
  type: integer
- description: The time when the cluster was last restarted, represented as epoch milliseconds.
  name: last_restarted_time
  type: integer
- description: The email address of the user who created the cluster.
  name: creator_user_name
  type: string
- description: The source that initiated the creation of this cluster.
  name: cluster_source
  type: string
- description: A map of Spark configuration key-value pairs that override the default Spark configuration values for this cluster.
  name: spark_conf
  type: object
- description: Additional tags applied to the cluster resources. Tags are propagated to the underlying cloud provider instances for cost tracking and resource management.
  name: custom_tags
  type: object
- description: Environment variables set for all Spark processes running on this cluster. Use the syntax {{secrets/scope/key}} to reference Databricks secrets.
  name: spark_env_vars
  type: object
- description: The number of minutes of inactivity after which the cluster is automatically terminated. A value of 0 disables auto-termination. Default is 120 minutes.
  name: autotermination_minutes
  type: integer
- description: Whether autoscaling local storage is enabled. When enabled, Databricks monitors disk usage on Spark workers and automatically attaches additional disks when needed.
  name: enable_elastic_disk
  type: boolean
- description: The ID of the instance pool to use for cluster nodes. Instance pools reduce cluster start time by maintaining idle, ready-to-use instances.
  name: instance_pool_id
  type:
  - string
  - 'null'
- description: The ID of the cluster policy applied to this cluster. Cluster policies constrain configuration settings and enforce organizational governance.
  name: policy_id
  type:
  - string
  - 'null'
- description: Whether data stored on local disks is encrypted.
  name: enable_local_disk_encryption
  type: boolean
- description: The data security mode of the cluster, which determines how data access is controlled.
  name: data_security_mode
  type: string
- description: The user name (email) of the single user when data_security_mode is SINGLE_USER.
  name: single_user_name
  type:
  - string
  - 'null'
- description: The runtime engine to use. PHOTON enables the Photon vectorized query engine for significantly faster performance on SQL and DataFrame workloads.
  name: runtime_engine
  type: string
- description: AWS-specific attributes for clusters running on Amazon Web Services.
  name: aws_attributes
  type:
  - object
  - 'null'
- description: Azure-specific attributes for clusters running on Microsoft Azure.
  name: azure_attributes
  type:
  - object
  - 'null'
- description: GCP-specific attributes for clusters running on Google Cloud Platform.
  name: gcp_attributes
  type:
  - object
  - 'null'
- description: Initialization scripts that run on each node when the cluster starts. Scripts can be stored in workspace files, Unity Catalog volumes, or DBFS.
  name: init_scripts
  type: array
- description: Default tags automatically applied by Databricks, including Vendor, Creator, ClusterName, and ClusterId.
  name: default_tags
  type: object
- description: The reason the cluster was terminated, including error codes and parameters.
  name: termination_reason
  type:
  - object
  - 'null'
- description: Information about the Spark driver node.
  name: driver
  type:
  - object
  - 'null'
- description: Information about the Spark executor (worker) nodes.
  name: executors
  type: array
- description: The port number on the driver node that serves JDBC/ODBC connections.
  name: jdbc_port
  type: integer
- description: The canonical Spark context identifier for this cluster.
  name: spark_context_id
  type: integer
- description: SSH public keys added to each Spark node in this cluster for SSH access.
  name: ssh_public_keys
  type: array
- description: Disk specifications for the cluster nodes.
  name: disk_spec
  type:
  - object
  - 'null'
- description: Status of cluster log delivery.
  name: cluster_log_status
  type:
  - object
  - 'null'
provider_name: Databricks
provider_slug: databricks
schema_file: json-schema/databricks-cluster-schema.json
slug: databricks-cluster
source_filename: databricks-cluster-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/databricks/refs/heads/main/json-schema/databricks-cluster-schema.json\",\n  \"title\": \"Databricks Cluster\",\n  \"description\": \"Schema representing a Databricks cluster, which is a managed cloud resource for running data engineering and data science workloads on Apache Spark. Clusters can be configured with fixed or autoscaling worker counts, various node types, and cloud-provider-specific attributes.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cluster_id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier assigned to the cluster by Databricks. This ID is generated during cluster creation and is used to reference the cluster in all subsequent API calls.\",\n      \"examples\": [\"1234-567890-abcde123\"]\n    },\n    \"cluster_name\": {\n      \"type\": \"string\",\n      \"description\": \"A human-readable\
  \ name for the cluster. This does not need to be unique within the workspace.\",\n      \"examples\": [\"my-data-cluster\"]\n    },\n    \"spark_version\": {\n      \"type\": \"string\",\n      \"description\": \"The Databricks Runtime version of the cluster, which determines the versions of Apache Spark, Scala, Java, Python, R, and installed libraries. Use the Runtime Versions API to retrieve available versions.\",\n      \"examples\": [\"14.3.x-scala2.12\", \"15.4.x-scala2.12\", \"14.3.x-photon-scala2.12\"]\n    },\n    \"node_type_id\": {\n      \"type\": \"string\",\n      \"description\": \"The cloud provider instance type for worker nodes. Determines the compute and memory resources available to each worker.\",\n      \"examples\": [\"i3.xlarge\", \"Standard_DS3_v2\", \"n1-standard-4\"]\n    },\n    \"driver_node_type_id\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The cloud provider instance type for the Spark driver node. If not specified, defaults to\
  \ the same value as node_type_id.\",\n      \"examples\": [\"i3.2xlarge\"]\n    },\n    \"num_workers\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of worker nodes in a fixed-size cluster. A cluster has one Spark driver and num_workers executors. Set to 0 for a single-node cluster where the driver acts as both driver and worker.\",\n      \"minimum\": 0,\n      \"examples\": [2, 8]\n    },\n    \"autoscale\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"Autoscaling configuration. When set, num_workers is ignored and the cluster dynamically scales between min_workers and max_workers based on workload.\",\n      \"properties\": {\n        \"min_workers\": {\n          \"type\": \"integer\",\n          \"description\": \"The minimum number of workers the cluster can scale down to when underutilized.\",\n          \"minimum\": 0\n        },\n        \"max_workers\": {\n          \"type\": \"integer\",\n          \"description\": \"The maximum\
  \ number of workers the cluster can scale up to under heavy load.\",\n          \"minimum\": 1\n        }\n      },\n      \"required\": [\"min_workers\", \"max_workers\"]\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"The current state of the cluster in its lifecycle.\",\n      \"enum\": [\n        \"PENDING\",\n        \"RUNNING\",\n        \"RESTARTING\",\n        \"RESIZING\",\n        \"TERMINATING\",\n        \"TERMINATED\",\n        \"ERROR\",\n        \"UNKNOWN\"\n      ]\n    },\n    \"state_message\": {\n      \"type\": \"string\",\n      \"description\": \"A human-readable message providing additional information about the current cluster state, such as the reason for termination.\"\n    },\n    \"start_time\": {\n      \"type\": \"integer\",\n      \"description\": \"The time when the cluster was started, represented as epoch milliseconds (Unix timestamp in milliseconds).\",\n      \"format\": \"int64\"\n    },\n    \"terminated_time\": {\n\
  \      \"type\": \"integer\",\n      \"description\": \"The time when the cluster was terminated, represented as epoch milliseconds.\",\n      \"format\": \"int64\"\n    },\n    \"last_state_loss_time\": {\n      \"type\": \"integer\",\n      \"description\": \"The time when the cluster driver last lost its state, represented as epoch milliseconds. This occurs when the driver node is lost or restarted.\",\n      \"format\": \"int64\"\n    },\n    \"last_activity_time\": {\n      \"type\": \"integer\",\n      \"description\": \"The time of the last user activity on the cluster, used for auto-termination calculations. Represented as epoch milliseconds.\",\n      \"format\": \"int64\"\n    },\n    \"last_restarted_time\": {\n      \"type\": \"integer\",\n      \"description\": \"The time when the cluster was last restarted, represented as epoch milliseconds.\",\n      \"format\": \"int64\"\n    },\n    \"creator_user_name\": {\n      \"type\": \"string\",\n      \"description\": \"The email\
  \ address of the user who created the cluster.\",\n      \"format\": \"email\"\n    },\n    \"cluster_source\": {\n      \"type\": \"string\",\n      \"description\": \"The source that initiated the creation of this cluster.\",\n      \"enum\": [\n        \"UI\",\n        \"API\",\n        \"JOB\",\n        \"MODELS\",\n        \"PIPELINE\",\n        \"PIPELINE_MAINTENANCE\",\n        \"SQL\",\n        \"SOME_OTHER_SOURCE\"\n      ]\n    },\n    \"spark_conf\": {\n      \"type\": \"object\",\n      \"description\": \"A map of Spark configuration key-value pairs that override the default Spark configuration values for this cluster.\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"examples\": [\n        {\n          \"spark.databricks.cluster.profile\": \"serverless\",\n          \"spark.speculation\": \"true\"\n        }\n      ]\n    },\n    \"custom_tags\": {\n      \"type\": \"object\",\n      \"description\": \"Additional tags applied to the cluster\
  \ resources. Tags are propagated to the underlying cloud provider instances for cost tracking and resource management.\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"examples\": [\n        {\n          \"team\": \"data-engineering\",\n          \"environment\": \"production\"\n        }\n      ]\n    },\n    \"spark_env_vars\": {\n      \"type\": \"object\",\n      \"description\": \"Environment variables set for all Spark processes running on this cluster. Use the syntax {{secrets/scope/key}} to reference Databricks secrets.\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"autotermination_minutes\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of minutes of inactivity after which the cluster is automatically terminated. A value of 0 disables auto-termination. Default is 120 minutes.\",\n      \"minimum\": 0,\n      \"default\": 120\n    },\n    \"enable_elastic_disk\": {\n      \"\
  type\": \"boolean\",\n      \"description\": \"Whether autoscaling local storage is enabled. When enabled, Databricks monitors disk usage on Spark workers and automatically attaches additional disks when needed.\"\n    },\n    \"instance_pool_id\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The ID of the instance pool to use for cluster nodes. Instance pools reduce cluster start time by maintaining idle, ready-to-use instances.\"\n    },\n    \"policy_id\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The ID of the cluster policy applied to this cluster. Cluster policies constrain configuration settings and enforce organizational governance.\"\n    },\n    \"enable_local_disk_encryption\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether data stored on local disks is encrypted.\"\n    },\n    \"data_security_mode\": {\n      \"type\": \"string\",\n      \"description\": \"The data security mode of the cluster, which determines\
  \ how data access is controlled.\",\n      \"enum\": [\n        \"NONE\",\n        \"SINGLE_USER\",\n        \"USER_ISOLATION\",\n        \"LEGACY_TABLE_ACL\",\n        \"LEGACY_PASSTHROUGH\",\n        \"LEGACY_SINGLE_USER\",\n        \"LEGACY_SINGLE_USER_STANDARD\"\n      ]\n    },\n    \"single_user_name\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The user name (email) of the single user when data_security_mode is SINGLE_USER.\",\n      \"format\": \"email\"\n    },\n    \"runtime_engine\": {\n      \"type\": \"string\",\n      \"description\": \"The runtime engine to use. PHOTON enables the Photon vectorized query engine for significantly faster performance on SQL and DataFrame workloads.\",\n      \"enum\": [\"STANDARD\", \"PHOTON\"]\n    },\n    \"aws_attributes\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"AWS-specific attributes for clusters running on Amazon Web Services.\",\n      \"properties\": {\n        \"first_on_demand\"\
  : {\n          \"type\": \"integer\",\n          \"description\": \"The number of nodes to place on on-demand instances before using spot instances.\"\n        },\n        \"availability\": {\n          \"type\": \"string\",\n          \"enum\": [\"SPOT\", \"ON_DEMAND\", \"SPOT_WITH_FALLBACK\"],\n          \"description\": \"The availability type for the cluster instances.\"\n        },\n        \"zone_id\": {\n          \"type\": \"string\",\n          \"description\": \"The AWS availability zone identifier.\"\n        },\n        \"instance_profile_arn\": {\n          \"type\": \"string\",\n          \"description\": \"The IAM instance profile ARN for the cluster EC2 instances.\"\n        },\n        \"spot_bid_price_percent\": {\n          \"type\": \"integer\",\n          \"description\": \"The max bid price for spot instances as a percentage of the on-demand price.\",\n          \"minimum\": 1,\n          \"maximum\": 10000\n        },\n        \"ebs_volume_type\": {\n          \"\
  type\": \"string\",\n          \"enum\": [\"GENERAL_PURPOSE_SSD\", \"THROUGHPUT_OPTIMIZED_HDD\"]\n        },\n        \"ebs_volume_count\": {\n          \"type\": \"integer\",\n          \"minimum\": 0\n        },\n        \"ebs_volume_size\": {\n          \"type\": \"integer\",\n          \"description\": \"The size of each EBS volume in GiB.\"\n        }\n      }\n    },\n    \"azure_attributes\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"Azure-specific attributes for clusters running on Microsoft Azure.\",\n      \"properties\": {\n        \"first_on_demand\": {\n          \"type\": \"integer\"\n        },\n        \"availability\": {\n          \"type\": \"string\",\n          \"enum\": [\"SPOT_AZURE\", \"ON_DEMAND_AZURE\", \"SPOT_WITH_FALLBACK_AZURE\"]\n        },\n        \"spot_bid_max_price\": {\n          \"type\": \"number\",\n          \"description\": \"The max bid price for Azure spot instances. -1 means the price is up to the on-demand price.\"\n\
  \        }\n      }\n    },\n    \"gcp_attributes\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"GCP-specific attributes for clusters running on Google Cloud Platform.\",\n      \"properties\": {\n        \"use_preemptible_executors\": {\n          \"type\": \"boolean\"\n        },\n        \"google_service_account\": {\n          \"type\": \"string\"\n        },\n        \"availability\": {\n          \"type\": \"string\",\n          \"enum\": [\"GCP_PREEMPTIBLE\", \"GCP_ON_DEMAND\"]\n        }\n      }\n    },\n    \"init_scripts\": {\n      \"type\": \"array\",\n      \"description\": \"Initialization scripts that run on each node when the cluster starts. Scripts can be stored in workspace files, Unity Catalog volumes, or DBFS.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"workspace\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"destination\": {\n                \"type\"\
  : \"string\",\n                \"description\": \"Workspace file path of the init script.\"\n              }\n            }\n          },\n          \"volumes\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"destination\": {\n                \"type\": \"string\",\n                \"description\": \"Unity Catalog volume path of the init script.\"\n              }\n            }\n          },\n          \"dbfs\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"destination\": {\n                \"type\": \"string\",\n                \"description\": \"DBFS path of the init script (deprecated).\"\n              }\n            },\n            \"deprecated\": true\n          }\n        }\n      }\n    },\n    \"default_tags\": {\n      \"type\": \"object\",\n      \"description\": \"Default tags automatically applied by Databricks, including Vendor, Creator, ClusterName, and ClusterId.\",\n      \"additionalProperties\"\
  : {\n        \"type\": \"string\"\n      }\n    },\n    \"termination_reason\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"The reason the cluster was terminated, including error codes and parameters.\",\n      \"properties\": {\n        \"code\": {\n          \"type\": \"string\",\n          \"description\": \"A machine-readable code indicating the termination reason.\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"The type of termination (e.g., CLIENT_ERROR, CLOUD_FAILURE).\"\n        },\n        \"parameters\": {\n          \"type\": \"object\",\n          \"additionalProperties\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"Additional parameters providing details about the termination.\"\n        }\n      }\n    },\n    \"driver\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"Information about the Spark driver node.\",\n      \"properties\": {\n   \
  \     \"private_ip\": {\n          \"type\": \"string\",\n          \"description\": \"The private IP address of the driver node.\"\n        },\n        \"public_dns\": {\n          \"type\": \"string\",\n          \"description\": \"The public DNS name of the driver node.\"\n        },\n        \"node_id\": {\n          \"type\": \"string\",\n          \"description\": \"The Databricks node identifier.\"\n        },\n        \"instance_id\": {\n          \"type\": \"string\",\n          \"description\": \"The cloud provider instance ID.\"\n        },\n        \"start_timestamp\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\"\n        },\n        \"host_private_ip\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"executors\": {\n      \"type\": \"array\",\n      \"description\": \"Information about the Spark executor (worker) nodes.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"private_ip\": {\n\
  \            \"type\": \"string\"\n          },\n          \"public_dns\": {\n            \"type\": \"string\"\n          },\n          \"node_id\": {\n            \"type\": \"string\"\n          },\n          \"instance_id\": {\n            \"type\": \"string\"\n          },\n          \"start_timestamp\": {\n            \"type\": \"integer\",\n            \"format\": \"int64\"\n          },\n          \"host_private_ip\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"jdbc_port\": {\n      \"type\": \"integer\",\n      \"description\": \"The port number on the driver node that serves JDBC/ODBC connections.\"\n    },\n    \"spark_context_id\": {\n      \"type\": \"integer\",\n      \"description\": \"The canonical Spark context identifier for this cluster.\",\n      \"format\": \"int64\"\n    },\n    \"ssh_public_keys\": {\n      \"type\": \"array\",\n      \"description\": \"SSH public keys added to each Spark node in this cluster for SSH access.\"\
  ,\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"disk_spec\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"Disk specifications for the cluster nodes.\",\n      \"properties\": {\n        \"disk_count\": {\n          \"type\": \"integer\",\n          \"description\": \"The number of disks attached to each node.\"\n        },\n        \"disk_size\": {\n          \"type\": \"integer\",\n          \"description\": \"The size of each disk in GiB.\"\n        },\n        \"disk_type\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"azure_disk_volume_type\": {\n              \"type\": \"string\"\n            },\n            \"ebs_volume_type\": {\n              \"type\": \"string\"\n            }\n          }\n        }\n      }\n    },\n    \"cluster_log_status\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"Status of cluster log delivery.\",\n      \"properties\": {\n        \"last_attempted\"\
  : {\n          \"type\": \"integer\",\n          \"format\": \"int64\",\n          \"description\": \"The timestamp of the last log delivery attempt.\"\n        },\n        \"last_exception\": {\n          \"type\": \"string\",\n          \"description\": \"The exception message if the last delivery attempt failed.\"\n        }\n      }\n    }\n  },\n  \"required\": [\"cluster_name\", \"spark_version\", \"node_type_id\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/databricks/refs/heads/main/json-schema/databricks-cluster-schema.json
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
title: Databricks Cluster
---
