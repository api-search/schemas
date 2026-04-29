---
description: Identity for the resource.
layout: schema
name: Identity
properties_list:
- description: The principal ID of resource identity.
  name: principalId
  type: string
- description: The tenant ID of resource.
  name: tenantId
  type: string
- description: The identity type.
  name: type
  type: string
provider_name: Azure Storage Account
provider_slug: azure-storage-account
schema_file: json-schema/azure-storage-account-identity-schema.json
slug: azure-storage-account-identity
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-storage-account/refs/heads/main/json-schema/azure-storage-account-identity-schema.json\",\n  \"title\": \"Identity\",\n  \"description\": \"Identity for the resource.\",\n  \"properties\": {\n    \"principalId\": {\n      \"description\": \"The principal ID of resource identity.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"tenantId\": {\n      \"description\": \"The tenant ID of resource.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"description\": \"The identity type.\",\n      \"enum\": [\n        \"SystemAssigned\"\n      ],\n      \"type\": \"string\",\n      \"x-ms-enum\": {\n        \"modelAsString\": false,\n        \"name\": \"IdentityType\"\n      }\n    }\n  },\n  \"type\": \"object\",\n  \"required\": [\n    \"type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-storage-account/refs/heads/main/json-schema/azure-storage-account-identity-schema.json
tags:
- Azure
- Blob Storage
- Cloud Storage
- File Storage
- Microsoft
- Storage
title: Identity
---
