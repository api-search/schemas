---
description: Description of site key vault references.
layout: schema
name: ApiKVReference
properties_list:
- description: ''
  name: details
  type: string
- description: ''
  name: identityType
  type: string
- description: ''
  name: location
  type: string
- description: ''
  name: reference
  type: string
- description: ''
  name: secretName
  type: string
- description: ''
  name: secretVersion
  type: string
- description: ''
  name: source
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: vaultName
  type: string
provider_name: Azure Functions
provider_slug: azure-functions
schema_file: json-schema/azure-functions-api-kv-reference-schema.json
slug: azure-functions-api-kv-reference
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-functions/refs/heads/main/json-schema/azure-functions-api-kv-reference-schema.json\",\n  \"title\": \"ApiKVReference\",\n  \"description\": \"Description of site key vault references.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"details\": {\n      \"type\": \"string\"\n    },\n    \"identityType\": {\n      \"enum\": [\n        \"None\",\n        \"SystemAssigned\",\n        \"UserAssigned\"\n      ],\n      \"type\": \"string\",\n      \"x-ms-enum\": {\n        \"modelAsString\": false,\n        \"name\": \"ManagedServiceIdentityType\"\n      }\n    },\n    \"location\": {\n      \"enum\": [\n        \"ApplicationSetting\"\n      ],\n      \"type\": \"string\",\n      \"x-ms-enum\": {\n        \"modelAsString\": false,\n        \"name\": \"ConfigReferenceLocation\"\n      }\n    },\n    \"reference\": {\n      \"type\": \"string\"\
  \n    },\n    \"secretName\": {\n      \"type\": \"string\"\n    },\n    \"secretVersion\": {\n      \"type\": \"string\"\n    },\n    \"source\": {\n      \"enum\": [\n        \"KeyVault\"\n      ],\n      \"type\": \"string\",\n      \"x-ms-enum\": {\n        \"modelAsString\": false,\n        \"name\": \"ConfigReferenceSource\"\n      }\n    },\n    \"status\": {\n      \"enum\": [\n        \"Initialized\",\n        \"Resolved\",\n        \"InvalidSyntax\",\n        \"MSINotEnabled\",\n        \"VaultNotFound\",\n        \"SecretNotFound\",\n        \"SecretVersionNotFound\",\n        \"AccessToKeyVaultDenied\",\n        \"OtherReasons\"\n      ],\n      \"type\": \"string\",\n      \"x-ms-enum\": {\n        \"modelAsString\": false,\n        \"name\": \"ResolveStatus\"\n      }\n    },\n    \"vaultName\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-functions/refs/heads/main/json-schema/azure-functions-api-kv-reference-schema.json
tags:
- Cloud
- Compute
- Event-Driven
- Functions
- Serverless
title: ApiKVReference
---
