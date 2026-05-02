---
description: An Apache Spark pool (Big Data pool) resource for big data processing workloads within a Synapse workspace.
layout: schema
name: Azure Synapse Analytics Spark Pool
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: type
  type: string
- description: The geo-location where the resource lives.
  name: location
  type: string
- description: ''
  name: tags
  type: object
- description: ''
  name: properties
  type: object
provider_name: Azure Synapse Analytics
provider_slug: microsoft-azure-synapse-analytics
schema_file: json-schema/azure-synapse-analytics-spark-pool-schema.json
slug: azure-synapse-analytics-spark-pool
source_filename: azure-synapse-analytics-spark-pool-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-search/azure-synapse-analytics/json-schema/azure-synapse-analytics-spark-pool-schema.json\",\n  \"title\": \"Azure Synapse Analytics Spark Pool\",\n  \"description\": \"An Apache Spark pool (Big Data pool) resource for big data processing workloads within a Synapse workspace.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"readOnly\": true\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"readOnly\": true\n    },\n    \"location\": {\n      \"type\": \"string\",\n      \"description\": \"The geo-location where the resource lives.\"\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"\
  provisioningState\": {\n          \"type\": \"string\",\n          \"readOnly\": true\n        },\n        \"autoScale\": {\n          \"$ref\": \"#/$defs/AutoScaleProperties\"\n        },\n        \"autoPause\": {\n          \"$ref\": \"#/$defs/AutoPauseProperties\"\n        },\n        \"sparkVersion\": {\n          \"type\": \"string\",\n          \"description\": \"The Apache Spark version.\"\n        },\n        \"nodeCount\": {\n          \"type\": \"integer\",\n          \"description\": \"The number of nodes in the Spark pool.\"\n        },\n        \"nodeSize\": {\n          \"type\": \"string\",\n          \"description\": \"The level of compute power.\",\n          \"enum\": [\"None\", \"Small\", \"Medium\", \"Large\", \"XLarge\", \"XXLarge\", \"XXXLarge\"]\n        },\n        \"nodeSizeFamily\": {\n          \"type\": \"string\",\n          \"description\": \"The kind of nodes that the Spark pool provides.\",\n          \"enum\": [\"None\", \"MemoryOptimized\", \"HardwareAcceleratedFPGA\"\
  , \"HardwareAcceleratedGPU\"]\n        },\n        \"sparkEventsFolder\": {\n          \"type\": \"string\",\n          \"description\": \"The Spark events folder.\"\n        },\n        \"defaultSparkLogFolder\": {\n          \"type\": \"string\",\n          \"description\": \"The default folder where Spark logs will be written.\"\n        },\n        \"isComputeIsolationEnabled\": {\n          \"type\": \"boolean\"\n        },\n        \"sessionLevelPackagesEnabled\": {\n          \"type\": \"boolean\"\n        },\n        \"dynamicExecutorAllocation\": {\n          \"$ref\": \"#/$defs/DynamicExecutorAllocation\"\n        },\n        \"creationDate\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"readOnly\": true\n        }\n      }\n    }\n  },\n  \"required\": [\"location\"],\n  \"$defs\": {\n    \"AutoScaleProperties\": {\n      \"type\": \"object\",\n      \"description\": \"Auto-scale configuration for the Spark pool.\",\n      \"properties\"\
  : {\n        \"minNodeCount\": {\n          \"type\": \"integer\",\n          \"description\": \"The minimum number of nodes the pool can scale to.\"\n        },\n        \"enabled\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether auto-scale is enabled.\"\n        },\n        \"maxNodeCount\": {\n          \"type\": \"integer\",\n          \"description\": \"The maximum number of nodes the pool can scale to.\"\n        }\n      }\n    },\n    \"AutoPauseProperties\": {\n      \"type\": \"object\",\n      \"description\": \"Auto-pause configuration for the Spark pool.\",\n      \"properties\": {\n        \"delayInMinutes\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of minutes of idle time before the pool is automatically paused.\"\n        },\n        \"enabled\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether auto-pause is enabled.\"\n        }\n      }\n    },\n    \"DynamicExecutorAllocation\": {\n \
  \     \"type\": \"object\",\n      \"description\": \"Dynamic executor allocation settings.\",\n      \"properties\": {\n        \"enabled\": {\n          \"type\": \"boolean\"\n        },\n        \"minExecutors\": {\n          \"type\": \"integer\"\n        },\n        \"maxExecutors\": {\n          \"type\": \"integer\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-synapse-analytics/refs/heads/main/json-schema/azure-synapse-analytics-spark-pool-schema.json
tags:
- Analytics
- Apache Spark
- Big Data
- Data Integration
- Data Warehouse
- ETL
- SQL
title: Azure Synapse Analytics Spark Pool
---
