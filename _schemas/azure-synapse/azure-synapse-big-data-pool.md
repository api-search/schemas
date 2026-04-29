---
description: An Apache Spark pool resource.
layout: schema
name: BigDataPool
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: location
  type: string
- description: ''
  name: properties
  type: object
provider_name: Azure Synapse Analytics
provider_slug: azure-synapse
schema_file: json-schema/azure-synapse-big-data-pool-schema.json
slug: azure-synapse-big-data-pool
source_filename: azure-synapse-big-data-pool-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-synapse/refs/heads/main/json-schema/azure-synapse-big-data-pool-schema.json\",\n  \"title\": \"BigDataPool\",\n  \"description\": \"An Apache Spark pool resource.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"readOnly\": true\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"readOnly\": true\n    },\n    \"location\": {\n      \"type\": \"string\"\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"provisioningState\": {\n          \"type\": \"string\",\n          \"readOnly\": true\n        },\n        \"nodeCount\": {\n          \"type\": \"integer\"\n        },\n        \"nodeSize\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"Small\",\n            \"Medium\",\n            \"Large\",\n           \
  \ \"XLarge\",\n            \"XXLarge\",\n            \"XXXLarge\"\n          ]\n        },\n        \"sparkVersion\": {\n          \"type\": \"string\"\n        },\n        \"autoScaleProperties\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"minNodeCount\": {\n              \"type\": \"integer\"\n            },\n            \"maxNodeCount\": {\n              \"type\": \"integer\"\n            },\n            \"enabled\": {\n              \"type\": \"boolean\"\n            }\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-synapse/refs/heads/main/json-schema/azure-synapse-big-data-pool-schema.json
tags:
- Analytics
- Apache Spark
- Big Data
- Data Warehouse
- ETL
- SQL
title: BigDataPool
---
