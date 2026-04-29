---
description: A SQL pool resource.
layout: schema
name: SqlPool
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
  name: tags
  type: object
- description: ''
  name: sku
  type: object
- description: ''
  name: properties
  type: object
provider_name: Azure Synapse Analytics
provider_slug: azure-synapse
schema_file: json-schema/azure-synapse-sql-pool-schema.json
slug: azure-synapse-sql-pool
source_filename: azure-synapse-sql-pool-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-synapse/refs/heads/main/json-schema/azure-synapse-sql-pool-schema.json\",\n  \"title\": \"SqlPool\",\n  \"description\": \"A SQL pool resource.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"readOnly\": true\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"readOnly\": true\n    },\n    \"location\": {\n      \"type\": \"string\"\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"sku\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"tier\": {\n          \"type\": \"string\"\n        },\n        \"name\": {\n          \"type\": \"string\"\n        },\n        \"capacity\": {\n          \"type\": \"integer\"\n        }\n      }\n    },\n    \"properties\": {\n    \
  \  \"type\": \"object\",\n      \"properties\": {\n        \"provisioningState\": {\n          \"type\": \"string\",\n          \"readOnly\": true\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"readOnly\": true\n        },\n        \"restorePointInTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-synapse/refs/heads/main/json-schema/azure-synapse-sql-pool-schema.json
tags:
- Analytics
- Apache Spark
- Big Data
- Data Warehouse
- ETL
- SQL
title: SqlPool
---
