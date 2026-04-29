---
description: WorkspaceInfoListResult schema from Azure Synapse Analytics API
layout: schema
name: WorkspaceInfoListResult
properties_list:
- description: ''
  name: value
  type: array
- description: ''
  name: nextLink
  type: string
provider_name: Azure Synapse Analytics
provider_slug: azure-synapse
schema_file: json-schema/azure-synapse-workspace-info-list-result-schema.json
slug: azure-synapse-workspace-info-list-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-synapse/refs/heads/main/json-schema/azure-synapse-workspace-info-list-result-schema.json\",\n  \"title\": \"WorkspaceInfoListResult\",\n  \"description\": \"WorkspaceInfoListResult schema from Azure Synapse Analytics API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"value\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Workspace\"\n      }\n    },\n    \"nextLink\": {\n      \"type\": \"string\",\n      \"readOnly\": true\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-synapse/refs/heads/main/json-schema/azure-synapse-workspace-info-list-result-schema.json
tags:
- Analytics
- Apache Spark
- Big Data
- Data Warehouse
- ETL
- SQL
title: WorkspaceInfoListResult
---
