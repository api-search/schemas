---
description: Schema representing an Azure Databricks cluster configuration and state. A cluster is a set of computation resources and configurations on which you run notebooks, jobs, and libraries. Clusters consist of a driver node and worker nodes running Apache Spark.
layout: schema
name: Azure Databricks Cluster
properties_list:
- description: Canonical identifier for the cluster, assigned by Databricks upon creation.
  name: cluster_id
  type: string
- description: Cluster name requested by the user. This name does not have to be unique. If not specified at creation, the cluster name defaults to an empty string.
  name: cluster_name
  type: string
- description: The Databricks Runtime version for the cluster. Determines the version of Apache Spark and other preinstalled libraries. Use the spark-versions API endpoint to retrieve available versions.
  name: spark_version
  type: string
- description: The Azure VM node type for worker nodes. Determines the amount of memory, CPU cores, and local storage available to each worker. Use the list-node-types API to retrieve available types.
  name: node_type_id
  type: string
- description: The Azure VM node type for the Spark driver node. If not specified, the driver node type defaults to the same value as node_type_id.
  name: driver_node_type_id
  type: string
- description: Number of worker nodes in the cluster. For a fixed-size cluster, set this to the desired number of workers. When autoscale is specified, this field is not used.
  name: num_workers
  type: integer
- description: Parameters for autoscaling the cluster. When specified, the cluster dynamically scales between the minimum and maximum number of workers based on workload.
  name: autoscale
  type: object
- description: An object containing a set of optional, user-specified Spark configuration key-value pairs. These are passed directly to the Spark driver and executors via the --conf flag.
  name: spark_conf
  type: object
- description: Attributes specific to Azure Databricks clusters, controlling Azure-specific behavior such as spot instance configuration.
  name: azure_attributes
  type: object
- description: SSH public key contents that are added to each node in the cluster. You can specify up to 10 keys.
  name: ssh_public_keys
  type: array
- description: Custom tags to apply to cluster resources. These tags are propagated to Azure resources created for the cluster. Databricks adds several default tags in addition to any custom tags specified.
  name: custom_tags
  type: object
- description: Configuration for delivering Spark logs to a long-term storage destination. Only one destination type can be specified.
  name: cluster_log_conf
  type: object
- description: Cluster-scoped init scripts to run when the cluster starts. Init scripts run before the Spark driver or workers start. A maximum of 10 init scripts can be specified.
  name: init_scripts
  type: array
- description: Environment variables to set on the Spark driver and worker processes. Key-value pairs are set as environment variables before the process starts.
  name: spark_env_vars
  type: object
- description: When enabled, the cluster will autoscale local storage. The disk space used by the cluster auto-adjusts based on the amount of data shuffled. Recommended for workloads with varying storage needs.
  name: enable_elastic_disk
  type: boolean
- description: The optional ID of the instance pool to use for cluster nodes. When specified, the cluster uses idle instances from the pool to reduce startup time. Both driver and worker nodes use the same pool unle
  name: instance_pool_id
  type: string
- description: The optional ID of the instance pool to use for the driver node. If specified, the driver uses this pool while workers use instance_pool_id.
  name: driver_instance_pool_id
  type: string
- description: Identifier of the cluster policy used to create the cluster. Cluster policies enforce configuration constraints and provide defaults.
  name: policy_id
  type: string
- description: When enabled, locally attached disks on cluster nodes are encrypted. This includes shuffle data, spilled data, and local caches.
  name: enable_local_disk_encryption
  type: boolean
- description: The runtime engine to use on the cluster. PHOTON provides a native vectorized query engine that accelerates SQL and DataFrame workloads.
  name: runtime_engine
  type: string
- description: The data security mode for the cluster. Controls how data access is governed. USER_ISOLATION provides per-user isolation with Unity Catalog. SINGLE_USER restricts the cluster to a single user.
  name: data_security_mode
  type: string
- description: The optional user name of the user assigned to the cluster when data_security_mode is SINGLE_USER. This user is the only one who can execute commands on the cluster.
  name: single_user_name
  type: string
- description: Current state of the cluster. PENDING indicates the cluster is being created; RUNNING means it is ready for use; TERMINATED means it has been stopped.
  name: state
  type: string
- description: A human-readable message providing additional details about the current state of the cluster.
  name: state_message
  type: string
- description: The username of the user who created the cluster.
  name: creator_user_name
  type: string
- description: Time (in epoch milliseconds) when the cluster was created or last started.
  name: start_time
  type: integer
- description: Time (in epoch milliseconds) when the cluster was terminated.
  name: terminated_time
  type: integer
- description: Time (in epoch milliseconds) when the cluster driver last lost its state. This occurs when the driver node is lost.
  name: last_state_loss_time
  type: integer
- description: Time (in epoch milliseconds) when the cluster last had activity. Inactivity duration is measured from this time for autotermination.
  name: last_activity_time
  type: integer
- description: Automatically terminates the cluster after it has been inactive for this time in minutes. If set to 0, the cluster is not auto-terminated. Default is 120 minutes.
  name: autotermination_minutes
  type: integer
- description: Indicates the source that created the cluster, such as UI, API, or JOB.
  name: cluster_source
  type: string
- description: Tags that are automatically applied by Databricks regardless of custom_tags settings. Includes Vendor, Creator, ClusterId, and ClusterName.
  name: default_tags
  type: object
- description: Information about why the cluster was terminated, available when the cluster is in TERMINATED state.
  name: termination_reason
  type: object
- description: Information about the Spark driver node.
  name: driver
  type: object
- description: Information about the Spark executor (worker) nodes.
  name: executors
  type: array
- description: Port on which the JDBC/ODBC server is listening for connections. Available only when the cluster is running.
  name: jdbc_port
  type: integer
- description: Total amount of memory (in megabytes) available across all nodes in the cluster.
  name: cluster_memory_mb
  type: integer
- description: Total number of CPU cores available across all nodes in the cluster.
  name: cluster_cores
  type: number
- description: Disk specification for the cluster nodes.
  name: disk_spec
  type: object
- description: Status of log delivery for the cluster.
  name: cluster_log_status
  type: object
provider_name: Azure Databricks
provider_slug: azure-databricks
schema_file: json-schema/azure-databricks-cluster-schema.json
slug: azure-databricks-cluster
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/kinlane/azure-databricks/json-schema/azure-databricks-cluster-schema.json\",\n  \"title\": \"Azure Databricks Cluster\",\n  \"description\": \"Schema representing an Azure Databricks cluster configuration and state. A cluster is a set of computation resources and configurations on which you run notebooks, jobs, and libraries. Clusters consist of a driver node and worker nodes running Apache Spark.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"spark_version\"\n  ],\n  \"properties\": {\n    \"cluster_id\": {\n      \"type\": \"string\",\n      \"description\": \"Canonical identifier for the cluster, assigned by Databricks upon creation.\",\n      \"examples\": [\n        \"1234-567890-abcde123\"\n      ]\n    },\n    \"cluster_name\": {\n      \"type\": \"string\",\n      \"description\": \"Cluster name requested by the user. This name does not have to be unique. If not\
  \ specified at creation, the cluster name defaults to an empty string.\",\n      \"examples\": [\n        \"my-analytics-cluster\"\n      ]\n    },\n    \"spark_version\": {\n      \"type\": \"string\",\n      \"description\": \"The Databricks Runtime version for the cluster. Determines the version of Apache Spark and other preinstalled libraries. Use the spark-versions API endpoint to retrieve available versions.\",\n      \"examples\": [\n        \"13.3.x-scala2.12\",\n        \"14.3.x-scala2.12\",\n        \"15.4.x-scala2.12\"\n      ]\n    },\n    \"node_type_id\": {\n      \"type\": \"string\",\n      \"description\": \"The Azure VM node type for worker nodes. Determines the amount of memory, CPU cores, and local storage available to each worker. Use the list-node-types API to retrieve available types.\",\n      \"examples\": [\n        \"Standard_DS3_v2\",\n        \"Standard_D4s_v3\",\n        \"Standard_E8s_v3\"\n      ]\n    },\n    \"driver_node_type_id\": {\n      \"type\":\
  \ \"string\",\n      \"description\": \"The Azure VM node type for the Spark driver node. If not specified, the driver node type defaults to the same value as node_type_id.\",\n      \"examples\": [\n        \"Standard_DS3_v2\",\n        \"Standard_D4s_v3\"\n      ]\n    },\n    \"num_workers\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"Number of worker nodes in the cluster. For a fixed-size cluster, set this to the desired number of workers. When autoscale is specified, this field is not used.\"\n    },\n    \"autoscale\": {\n      \"type\": \"object\",\n      \"description\": \"Parameters for autoscaling the cluster. When specified, the cluster dynamically scales between the minimum and maximum number of workers based on workload.\",\n      \"required\": [\n        \"min_workers\",\n        \"max_workers\"\n      ],\n      \"properties\": {\n        \"min_workers\": {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"description\"\
  : \"The minimum number of workers the cluster can scale down to when underutilized. The cluster will not go below this number of nodes.\"\n        },\n        \"max_workers\": {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"description\": \"The maximum number of workers the cluster can scale up to when the workload requires more resources.\"\n        }\n      },\n      \"additionalProperties\": false\n    },\n    \"spark_conf\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"An object containing a set of optional, user-specified Spark configuration key-value pairs. These are passed directly to the Spark driver and executors via the --conf flag.\",\n      \"examples\": [\n        {\n          \"spark.speculation\": \"true\",\n          \"spark.streaming.ui.retainedBatches\": \"5\"\n        }\n      ]\n    },\n    \"azure_attributes\": {\n      \"type\": \"object\",\n      \"\
  description\": \"Attributes specific to Azure Databricks clusters, controlling Azure-specific behavior such as spot instance configuration.\",\n      \"properties\": {\n        \"first_on_demand\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"The first nodes in the cluster that are provisioned as on-demand instances. The rest are provisioned as spot (preemptible) instances. Set to 0 for all spot, or equal to num_workers for all on-demand.\"\n        },\n        \"availability\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"SPOT_AZURE\",\n            \"ON_DEMAND_AZURE\",\n            \"SPOT_WITH_FALLBACK_AZURE\"\n          ],\n          \"description\": \"The Azure availability type for the worker nodes. SPOT_WITH_FALLBACK_AZURE uses spot instances when available and falls back to on-demand.\"\n        },\n        \"spot_bid_max_price\": {\n          \"type\": \"number\",\n          \"description\": \"The max price\
  \ for Azure spot instances. Set to -1 (the default) to indicate that the instance should not be evicted on the basis of price. The spot price for the instance will be the current price for spot instances or the price for a standard instance if lower.\"\n        }\n      },\n      \"additionalProperties\": false\n    },\n    \"ssh_public_keys\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"SSH public key contents that are added to each node in the cluster. You can specify up to 10 keys.\"\n    },\n    \"custom_tags\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Custom tags to apply to cluster resources. These tags are propagated to Azure resources created for the cluster. Databricks adds several default tags in addition to any custom tags specified.\",\n      \"examples\": [\n        {\n          \"Environment\": \"Production\",\n\
  \          \"Team\": \"Data Engineering\",\n          \"CostCenter\": \"12345\"\n        }\n      ]\n    },\n    \"cluster_log_conf\": {\n      \"type\": \"object\",\n      \"description\": \"Configuration for delivering Spark logs to a long-term storage destination. Only one destination type can be specified.\",\n      \"properties\": {\n        \"dbfs\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"destination\": {\n              \"type\": \"string\",\n              \"description\": \"DBFS destination path for cluster logs, e.g., dbfs:/cluster-logs.\",\n              \"examples\": [\n                \"dbfs:/cluster-logs\"\n              ]\n            }\n          },\n          \"required\": [\n            \"destination\"\n          ],\n          \"additionalProperties\": false\n        },\n        \"s3\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"destination\": {\n              \"type\": \"string\",\n           \
  \   \"description\": \"S3 destination URI for cluster logs.\"\n            },\n            \"region\": {\n              \"type\": \"string\",\n              \"description\": \"S3 region, e.g., us-west-2.\"\n            },\n            \"endpoint\": {\n              \"type\": \"string\",\n              \"description\": \"S3 endpoint URL.\"\n            }\n          },\n          \"required\": [\n            \"destination\"\n          ],\n          \"additionalProperties\": false\n        }\n      },\n      \"additionalProperties\": false\n    },\n    \"init_scripts\": {\n      \"type\": \"array\",\n      \"description\": \"Cluster-scoped init scripts to run when the cluster starts. Init scripts run before the Spark driver or workers start. A maximum of 10 init scripts can be specified.\",\n      \"maxItems\": 10,\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"An init script source definition. Exactly one of the destination types must be specified.\",\n  \
  \      \"properties\": {\n          \"workspace\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"destination\": {\n                \"type\": \"string\",\n                \"description\": \"Workspace filesystem path to the init script.\",\n                \"examples\": [\n                  \"/Workspace/init-scripts/my-init.sh\"\n                ]\n              }\n            },\n            \"required\": [\n              \"destination\"\n            ],\n            \"additionalProperties\": false\n          },\n          \"volumes\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"destination\": {\n                \"type\": \"string\",\n                \"description\": \"Unity Catalog Volumes path to the init script.\",\n                \"examples\": [\n                  \"/Volumes/my_catalog/my_schema/my_volume/init.sh\"\n                ]\n              }\n            },\n            \"required\": [\n       \
  \       \"destination\"\n            ],\n            \"additionalProperties\": false\n          },\n          \"dbfs\": {\n            \"type\": \"object\",\n            \"deprecated\": true,\n            \"properties\": {\n              \"destination\": {\n                \"type\": \"string\",\n                \"description\": \"DBFS path to the init script. Deprecated: use workspace or volumes instead.\"\n              }\n            },\n            \"required\": [\n              \"destination\"\n            ],\n            \"additionalProperties\": false\n          },\n          \"abfss\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"destination\": {\n                \"type\": \"string\",\n                \"description\": \"Azure Blob Filesystem (ABFSS) path to the init script.\"\n              }\n            },\n            \"required\": [\n              \"destination\"\n            ],\n            \"additionalProperties\": false\n          }\n\
  \        },\n        \"additionalProperties\": false\n      }\n    },\n    \"spark_env_vars\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Environment variables to set on the Spark driver and worker processes. Key-value pairs are set as environment variables before the process starts.\",\n      \"examples\": [\n        {\n          \"PYSPARK_PYTHON\": \"/databricks/python3/bin/python3\"\n        }\n      ]\n    },\n    \"enable_elastic_disk\": {\n      \"type\": \"boolean\",\n      \"description\": \"When enabled, the cluster will autoscale local storage. The disk space used by the cluster auto-adjusts based on the amount of data shuffled. Recommended for workloads with varying storage needs.\",\n      \"default\": false\n    },\n    \"instance_pool_id\": {\n      \"type\": \"string\",\n      \"description\": \"The optional ID of the instance pool to use for cluster nodes. When specified, the cluster\
  \ uses idle instances from the pool to reduce startup time. Both driver and worker nodes use the same pool unless driver_instance_pool_id is also set.\"\n    },\n    \"driver_instance_pool_id\": {\n      \"type\": \"string\",\n      \"description\": \"The optional ID of the instance pool to use for the driver node. If specified, the driver uses this pool while workers use instance_pool_id.\"\n    },\n    \"policy_id\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the cluster policy used to create the cluster. Cluster policies enforce configuration constraints and provide defaults.\"\n    },\n    \"enable_local_disk_encryption\": {\n      \"type\": \"boolean\",\n      \"description\": \"When enabled, locally attached disks on cluster nodes are encrypted. This includes shuffle data, spilled data, and local caches.\",\n      \"default\": false\n    },\n    \"runtime_engine\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"STANDARD\",\n        \"PHOTON\"\
  \n      ],\n      \"description\": \"The runtime engine to use on the cluster. PHOTON provides a native vectorized query engine that accelerates SQL and DataFrame workloads.\"\n    },\n    \"data_security_mode\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"NONE\",\n        \"SINGLE_USER\",\n        \"USER_ISOLATION\",\n        \"LEGACY_TABLE_ACL\",\n        \"LEGACY_PASSTHROUGH\",\n        \"LEGACY_SINGLE_USER\",\n        \"LEGACY_SINGLE_USER_STANDARD\"\n      ],\n      \"description\": \"The data security mode for the cluster. Controls how data access is governed. USER_ISOLATION provides per-user isolation with Unity Catalog. SINGLE_USER restricts the cluster to a single user.\"\n    },\n    \"single_user_name\": {\n      \"type\": \"string\",\n      \"description\": \"The optional user name of the user assigned to the cluster when data_security_mode is SINGLE_USER. This user is the only one who can execute commands on the cluster.\"\n    },\n    \"state\": {\n      \"\
  type\": \"string\",\n      \"enum\": [\n        \"PENDING\",\n        \"RUNNING\",\n        \"RESTARTING\",\n        \"RESIZING\",\n        \"TERMINATING\",\n        \"TERMINATED\",\n        \"ERROR\",\n        \"UNKNOWN\"\n      ],\n      \"description\": \"Current state of the cluster. PENDING indicates the cluster is being created; RUNNING means it is ready for use; TERMINATED means it has been stopped.\",\n      \"readOnly\": true\n    },\n    \"state_message\": {\n      \"type\": \"string\",\n      \"description\": \"A human-readable message providing additional details about the current state of the cluster.\",\n      \"readOnly\": true\n    },\n    \"creator_user_name\": {\n      \"type\": \"string\",\n      \"description\": \"The username of the user who created the cluster.\",\n      \"readOnly\": true\n    },\n    \"start_time\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Time (in epoch milliseconds) when the cluster was created or\
  \ last started.\",\n      \"readOnly\": true\n    },\n    \"terminated_time\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Time (in epoch milliseconds) when the cluster was terminated.\",\n      \"readOnly\": true\n    },\n    \"last_state_loss_time\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Time (in epoch milliseconds) when the cluster driver last lost its state. This occurs when the driver node is lost.\",\n      \"readOnly\": true\n    },\n    \"last_activity_time\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Time (in epoch milliseconds) when the cluster last had activity. Inactivity duration is measured from this time for autotermination.\",\n      \"readOnly\": true\n    },\n    \"autotermination_minutes\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"Automatically terminates the cluster after it has been inactive\
  \ for this time in minutes. If set to 0, the cluster is not auto-terminated. Default is 120 minutes.\",\n      \"default\": 120\n    },\n    \"cluster_source\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"UI\",\n        \"API\",\n        \"JOB\",\n        \"MODELS\",\n        \"PIPELINE\",\n        \"PIPELINE_MAINTENANCE\",\n        \"SQL\"\n      ],\n      \"description\": \"Indicates the source that created the cluster, such as UI, API, or JOB.\",\n      \"readOnly\": true\n    },\n    \"default_tags\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Tags that are automatically applied by Databricks regardless of custom_tags settings. Includes Vendor, Creator, ClusterId, and ClusterName.\",\n      \"readOnly\": true\n    },\n    \"termination_reason\": {\n      \"type\": \"object\",\n      \"description\": \"Information about why the cluster was terminated, available when the cluster\
  \ is in TERMINATED state.\",\n      \"properties\": {\n        \"code\": {\n          \"type\": \"string\",\n          \"description\": \"A status code indicating the reason for termination, such as INACTIVITY, USER_REQUEST, or CLOUD_FAILURE.\",\n          \"examples\": [\n            \"INACTIVITY\",\n            \"USER_REQUEST\",\n            \"CLOUD_FAILURE\",\n            \"INIT_SCRIPT_FAILURE\"\n          ]\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"SUCCESS\",\n            \"CLIENT_ERROR\",\n            \"SERVICE_FAULT\",\n            \"CLOUD_FAILURE\"\n          ],\n          \"description\": \"The general category of the termination reason.\"\n        },\n        \"parameters\": {\n          \"type\": \"object\",\n          \"additionalProperties\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"Additional parameters providing more details about the termination.\"\n        }\n      },\n\
  \      \"readOnly\": true,\n      \"additionalProperties\": false\n    },\n    \"driver\": {\n      \"type\": \"object\",\n      \"description\": \"Information about the Spark driver node.\",\n      \"properties\": {\n        \"private_ip\": {\n          \"type\": \"string\",\n          \"description\": \"Private IP address of the driver node.\"\n        },\n        \"public_dns\": {\n          \"type\": \"string\",\n          \"description\": \"Public DNS name of the driver node.\"\n        },\n        \"node_id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier for the driver node.\"\n        },\n        \"instance_id\": {\n          \"type\": \"string\",\n          \"description\": \"Azure instance identifier.\"\n        },\n        \"start_timestamp\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\",\n          \"description\": \"Start time of the driver node in epoch milliseconds.\"\n        },\n        \"host_private_ip\": {\n\
  \          \"type\": \"string\",\n          \"description\": \"Private IP address of the host machine.\"\n        }\n      },\n      \"readOnly\": true,\n      \"additionalProperties\": false\n    },\n    \"executors\": {\n      \"type\": \"array\",\n      \"description\": \"Information about the Spark executor (worker) nodes.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"private_ip\": {\n            \"type\": \"string\",\n            \"description\": \"Private IP address of the executor node.\"\n          },\n          \"public_dns\": {\n            \"type\": \"string\",\n            \"description\": \"Public DNS name of the executor node.\"\n          },\n          \"node_id\": {\n            \"type\": \"string\",\n            \"description\": \"Unique identifier for the executor node.\"\n          },\n          \"instance_id\": {\n            \"type\": \"string\",\n            \"description\": \"Azure instance identifier.\"\n         \
  \ },\n          \"start_timestamp\": {\n            \"type\": \"integer\",\n            \"format\": \"int64\",\n            \"description\": \"Start time of the executor node in epoch milliseconds.\"\n          },\n          \"host_private_ip\": {\n            \"type\": \"string\",\n            \"description\": \"Private IP address of the host machine.\"\n          }\n        },\n        \"additionalProperties\": false\n      },\n      \"readOnly\": true\n    },\n    \"jdbc_port\": {\n      \"type\": \"integer\",\n      \"description\": \"Port on which the JDBC/ODBC server is listening for connections. Available only when the cluster is running.\",\n      \"readOnly\": true\n    },\n    \"cluster_memory_mb\": {\n      \"type\": \"integer\",\n      \"description\": \"Total amount of memory (in megabytes) available across all nodes in the cluster.\",\n      \"readOnly\": true\n    },\n    \"cluster_cores\": {\n      \"type\": \"number\",\n      \"description\": \"Total number of CPU cores\
  \ available across all nodes in the cluster.\",\n      \"readOnly\": true\n    },\n    \"disk_spec\": {\n      \"type\": \"object\",\n      \"description\": \"Disk specification for the cluster nodes.\",\n      \"properties\": {\n        \"disk_count\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"Number of disks attached to each node.\"\n        },\n        \"disk_size\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"Size of each disk in gigabytes.\"\n        },\n        \"disk_type\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"azure_disk_volume_type\": {\n              \"type\": \"string\",\n              \"enum\": [\n                \"PREMIUM_LRS\",\n                \"STANDARD_LRS\"\n              ],\n              \"description\": \"Azure disk volume type. PREMIUM_LRS provides SSD-backed storage, STANDARD_LRS provides HDD-backed storage.\"\n           \
  \ }\n          },\n          \"additionalProperties\": false\n        }\n      },\n      \"additionalProperties\": false\n    },\n    \"cluster_log_status\": {\n      \"type\": \"object\",\n      \"description\": \"Status of log delivery for the cluster.\",\n      \"properties\": {\n        \"last_attempted\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\",\n          \"description\": \"Timestamp of the last attempted log delivery in epoch milliseconds.\"\n        },\n        \"last_exception\": {\n          \"type\": \"string\",\n          \"description\": \"Error message from the last failed log delivery attempt.\"\n        }\n      },\n      \"readOnly\": true,\n      \"additionalProperties\": false\n    }\n  },\n  \"additionalProperties\": false,\n  \"examples\": [\n    {\n      \"cluster_id\": \"1234-567890-abcde123\",\n      \"cluster_name\": \"my-analytics-cluster\",\n      \"spark_version\": \"14.3.x-scala2.12\",\n      \"node_type_id\": \"Standard_DS3_v2\"\
  ,\n      \"driver_node_type_id\": \"Standard_DS3_v2\",\n      \"autoscale\": {\n        \"min_workers\": 2,\n        \"max_workers\": 8\n      },\n      \"azure_attributes\": {\n        \"first_on_demand\": 1,\n        \"availability\": \"SPOT_WITH_FALLBACK_AZURE\",\n        \"spot_bid_max_price\": -1\n      },\n      \"spark_conf\": {\n        \"spark.databricks.delta.preview.enabled\": \"true\"\n      },\n      \"custom_tags\": {\n        \"Environment\": \"Production\",\n        \"Team\": \"Data Engineering\"\n      },\n      \"autotermination_minutes\": 120,\n      \"enable_elastic_disk\": true,\n      \"data_security_mode\": \"USER_ISOLATION\",\n      \"runtime_engine\": \"PHOTON\",\n      \"state\": \"RUNNING\",\n      \"state_message\": \"\",\n      \"creator_user_name\": \"user@example.com\",\n      \"start_time\": 1709472000000,\n      \"cluster_source\": \"API\"\n    }\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-databricks/refs/heads/main/json-schema/azure-databricks-cluster-schema.json
tags:
- Analytics
- Apache Spark
- Big Data
- Data Engineering
- Machine Learning
title: Azure Databricks Cluster
---
