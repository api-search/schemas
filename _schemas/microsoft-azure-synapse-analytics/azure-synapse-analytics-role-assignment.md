---
description: A role assignment that grants access to Synapse workspace resources through role-based access control.
layout: schema
name: Azure Synapse Analytics Role Assignment
properties_list:
- description: Role Assignment ID.
  name: id
  type: string
- description: Role Definition ID.
  name: roleDefinitionId
  type: string
- description: Object ID of the AAD principal or security-group.
  name: principalId
  type: string
- description: Scope at which the role assignment is created.
  name: scope
  type: string
- description: Type of the principal.
  name: principalType
  type: string
provider_name: Azure Synapse Analytics
provider_slug: microsoft-azure-synapse-analytics
schema_file: json-schema/azure-synapse-analytics-role-assignment-schema.json
slug: azure-synapse-analytics-role-assignment
source_filename: azure-synapse-analytics-role-assignment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-search/azure-synapse-analytics/json-schema/azure-synapse-analytics-role-assignment-schema.json\",\n  \"title\": \"Azure Synapse Analytics Role Assignment\",\n  \"description\": \"A role assignment that grants access to Synapse workspace resources through role-based access control.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Role Assignment ID.\"\n    },\n    \"roleDefinitionId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Role Definition ID.\"\n    },\n    \"principalId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Object ID of the AAD principal or security-group.\"\n    },\n    \"scope\": {\n      \"type\": \"string\",\n      \"description\": \"Scope at which the role assignment is created.\"\n    },\n    \"principalType\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Type of the principal.\",\n      \"enum\": [\"User\", \"Group\", \"ServicePrincipal\"]\n    }\n  },\n  \"required\": [\"roleDefinitionId\", \"principalId\", \"scope\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-synapse-analytics/refs/heads/main/json-schema/azure-synapse-analytics-role-assignment-schema.json
tags:
- Analytics
- Apache Spark
- Big Data
- Data Integration
- Data Warehouse
- ETL
- SQL
title: Azure Synapse Analytics Role Assignment
---
