---
description: A workspace resource.
layout: schema
name: Workspace
properties_list:
- description: Resource ID
  name: id
  type: string
- description: Resource name
  name: name
  type: string
- description: Resource type
  name: type
  type: string
- description: Azure region location
  name: location
  type: string
- description: Resource tags
  name: tags
  type: object
- description: ''
  name: properties
  type: object
provider_name: Azure Synapse Analytics
provider_slug: azure-synapse
schema_file: json-schema/azure-synapse-workspace-schema.json
slug: azure-synapse-workspace
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-synapse/refs/heads/main/json-schema/azure-synapse-workspace-schema.json\",\n  \"title\": \"Workspace\",\n  \"description\": \"A workspace resource.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"readOnly\": true,\n      \"description\": \"Resource ID\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"readOnly\": true,\n      \"description\": \"Resource name\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"readOnly\": true,\n      \"description\": \"Resource type\"\n    },\n    \"location\": {\n      \"type\": \"string\",\n      \"description\": \"Azure region location\"\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Resource tags\"\n    },\n    \"properties\"\
  : {\n      \"type\": \"object\",\n      \"properties\": {\n        \"provisioningState\": {\n          \"type\": \"string\",\n          \"readOnly\": true,\n          \"description\": \"Resource provisioning state\"\n        },\n        \"sqlAdministratorLogin\": {\n          \"type\": \"string\",\n          \"description\": \"SQL admin login name\"\n        },\n        \"defaultDataLakeStorage\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"accountUrl\": {\n              \"type\": \"string\"\n            },\n            \"filesystem\": {\n              \"type\": \"string\"\n            }\n          }\n        },\n        \"connectivityEndpoints\": {\n          \"type\": \"object\",\n          \"readOnly\": true,\n          \"additionalProperties\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-synapse/refs/heads/main/json-schema/azure-synapse-workspace-schema.json
tags:
- Analytics
- Apache Spark
- Big Data
- Data Warehouse
- ETL
- SQL
title: Workspace
---
