---
description: A dedicated SQL pool resource for enterprise data warehousing workloads within a Synapse workspace.
layout: schema
name: Azure Synapse Analytics SQL Pool
properties_list:
- description: Fully qualified resource ID.
  name: id
  type: string
- description: The name of the SQL pool.
  name: name
  type: string
- description: The type of the resource.
  name: type
  type: string
- description: The geo-location where the resource lives.
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
provider_slug: microsoft-azure-synapse-analytics
schema_file: json-schema/azure-synapse-analytics-sql-pool-schema.json
slug: azure-synapse-analytics-sql-pool
source_filename: azure-synapse-analytics-sql-pool-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-search/azure-synapse-analytics/json-schema/azure-synapse-analytics-sql-pool-schema.json\",\n  \"title\": \"Azure Synapse Analytics SQL Pool\",\n  \"description\": \"A dedicated SQL pool resource for enterprise data warehousing workloads within a Synapse workspace.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Fully qualified resource ID.\",\n      \"readOnly\": true\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the SQL pool.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the resource.\",\n      \"readOnly\": true\n    },\n    \"location\": {\n      \"type\": \"string\",\n      \"description\": \"The geo-location where the resource lives.\"\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"additionalProperties\"\
  : {\n        \"type\": \"string\"\n      }\n    },\n    \"sku\": {\n      \"$ref\": \"#/$defs/Sku\"\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"maxSizeBytes\": {\n          \"type\": \"integer\",\n          \"description\": \"Maximum size in bytes.\"\n        },\n        \"collation\": {\n          \"type\": \"string\",\n          \"description\": \"Collation mode for the SQL pool.\"\n        },\n        \"sourceDatabaseId\": {\n          \"type\": \"string\",\n          \"description\": \"Source database ID to create from.\"\n        },\n        \"recoverableDatabaseId\": {\n          \"type\": \"string\",\n          \"description\": \"Recoverable database ID for geo-restore.\"\n        },\n        \"provisioningState\": {\n          \"type\": \"string\",\n          \"description\": \"Resource provisioning state.\",\n          \"readOnly\": true\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"description\"\
  : \"Resource status.\",\n          \"readOnly\": true\n        },\n        \"restorePointInTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Snapshot time to restore from.\"\n        },\n        \"createMode\": {\n          \"type\": \"string\",\n          \"description\": \"Specifies the mode of SQL pool creation.\",\n          \"enum\": [\"Default\", \"PointInTimeRestore\", \"Recovery\", \"Restore\"]\n        },\n        \"creationDate\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"readOnly\": true\n        },\n        \"storageAccountType\": {\n          \"type\": \"string\",\n          \"description\": \"The storage account type for backup.\",\n          \"enum\": [\"GRS\", \"LRS\"]\n        }\n      }\n    }\n  },\n  \"required\": [\"location\"],\n  \"$defs\": {\n    \"Sku\": {\n      \"type\": \"object\",\n      \"description\": \"SQL pool SKU defining the performance tier.\",\n\
  \      \"properties\": {\n        \"tier\": {\n          \"type\": \"string\",\n          \"description\": \"The service tier.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The SKU name (e.g., DW100c, DW200c).\"\n        },\n        \"capacity\": {\n          \"type\": \"integer\",\n          \"description\": \"The SKU capacity.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-synapse-analytics/refs/heads/main/json-schema/azure-synapse-analytics-sql-pool-schema.json
tags:
- Analytics
- Apache Spark
- Big Data
- Data Integration
- Data Warehouse
- ETL
- SQL
title: Azure Synapse Analytics SQL Pool
---
