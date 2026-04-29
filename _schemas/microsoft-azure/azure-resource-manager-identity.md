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
- description: The list of user-assigned identities.
  name: userAssignedIdentities
  type: object
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-resource-manager-identity-schema.json
slug: azure-resource-manager-identity
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Identity\",\n  \"type\": \"object\",\n  \"description\": \"Identity for the resource.\",\n  \"properties\": {\n    \"principalId\": {\n      \"type\": \"string\",\n      \"description\": \"The principal ID of resource identity.\"\n    },\n    \"tenantId\": {\n      \"type\": \"string\",\n      \"description\": \"The tenant ID of resource.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The identity type.\"\n    },\n    \"userAssignedIdentities\": {\n      \"type\": \"object\",\n      \"description\": \"The list of user-assigned identities.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-resource-manager-identity-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: Identity
---
