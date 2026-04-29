---
description: User-assigned managed identity.
layout: schema
name: UserAssignedIdentity
properties_list:
- description: The principal ID of the user-assigned identity.
  name: principalId
  type: string
- description: The client ID of the user-assigned identity.
  name: clientId
  type: string
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-resource-manager-user-assigned-identity-schema.json
slug: azure-resource-manager-user-assigned-identity
source_filename: azure-resource-manager-user-assigned-identity-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UserAssignedIdentity\",\n  \"type\": \"object\",\n  \"description\": \"User-assigned managed identity.\",\n  \"properties\": {\n    \"principalId\": {\n      \"type\": \"string\",\n      \"description\": \"The principal ID of the user-assigned identity.\"\n    },\n    \"clientId\": {\n      \"type\": \"string\",\n      \"description\": \"The client ID of the user-assigned identity.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-resource-manager-user-assigned-identity-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: UserAssignedIdentity
---
