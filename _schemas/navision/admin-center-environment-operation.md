---
description: ''
layout: schema
name: EnvironmentOperation
properties_list:
- description: Operation ID used for tracking
  name: id
  type: string
- description: Type of operation
  name: type
  type: string
- description: Status of the operation
  name: status
  type: string
- description: Microsoft Entra tenant ID
  name: aadTenantId
  type: string
- description: When the operation was created
  name: createdOn
  type: string
- description: When the operation started executing
  name: startedOn
  type: string
- description: When the operation completed
  name: completedOn
  type: string
- description: Who created the operation
  name: createdBy
  type: string
- description: Error message for failed operations
  name: errorMessage
  type: string
- description: Operation-specific parameters
  name: parameters
  type: object
- description: Name of the affected environment
  name: environmentName
  type: string
- description: Type of the affected environment
  name: environmentType
  type: string
- description: Product family of the affected environment
  name: productFamily
  type: string
provider_name: Microsoft Dynamics NAV
provider_slug: navision
schema_file: json-schema/admin-center-environment-operation-schema.json
slug: admin-center-environment-operation
source_filename: admin-center-environment-operation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EnvironmentOperation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Operation ID used for tracking\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of operation\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Status of the operation\"\n    },\n    \"aadTenantId\": {\n      \"type\": \"string\",\n      \"description\": \"Microsoft Entra tenant ID\"\n    },\n    \"createdOn\": {\n      \"type\": \"string\",\n      \"description\": \"When the operation was created\"\n    },\n    \"startedOn\": {\n      \"type\": \"string\",\n      \"description\": \"When the operation started executing\"\n    },\n    \"completedOn\": {\n      \"type\": \"string\",\n      \"description\": \"When the operation completed\"\n    },\n    \"createdBy\": {\n      \"type\": \"\
  string\",\n      \"description\": \"Who created the operation\"\n    },\n    \"errorMessage\": {\n      \"type\": \"string\",\n      \"description\": \"Error message for failed operations\"\n    },\n    \"parameters\": {\n      \"type\": \"object\",\n      \"description\": \"Operation-specific parameters\"\n    },\n    \"environmentName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the affected environment\"\n    },\n    \"environmentType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of the affected environment\"\n    },\n    \"productFamily\": {\n      \"type\": \"string\",\n      \"description\": \"Product family of the affected environment\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/navision/refs/heads/main/json-schema/admin-center-environment-operation-schema.json
tags:
- Business Management
- Dynamics NAV
- ERP
- Finance
- Inventory
- Microsoft
- Navision
title: EnvironmentOperation
---
