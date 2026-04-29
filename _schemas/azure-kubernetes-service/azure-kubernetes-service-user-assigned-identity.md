---
description: Details about a user assigned identity.
layout: schema
name: UserAssignedIdentity
properties_list:
- description: The resource ID of the user assigned identity.
  name: resourceId
  type: string
- description: The client ID of the user assigned identity.
  name: clientId
  type: string
- description: The object ID of the user assigned identity.
  name: objectId
  type: string
provider_name: Azure Kubernetes Service
provider_slug: azure-kubernetes-service
schema_file: json-schema/azure-kubernetes-service-user-assigned-identity-schema.json
slug: azure-kubernetes-service-user-assigned-identity
source_filename: azure-kubernetes-service-user-assigned-identity-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UserAssignedIdentity\",\n  \"type\": \"object\",\n  \"description\": \"Details about a user assigned identity.\",\n  \"properties\": {\n    \"resourceId\": {\n      \"type\": \"string\",\n      \"description\": \"The resource ID of the user assigned identity.\"\n    },\n    \"clientId\": {\n      \"type\": \"string\",\n      \"description\": \"The client ID of the user assigned identity.\"\n    },\n    \"objectId\": {\n      \"type\": \"string\",\n      \"description\": \"The object ID of the user assigned identity.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-kubernetes-service/refs/heads/main/json-schema/azure-kubernetes-service-user-assigned-identity-schema.json
tags:
- Azure
- Cloud
- Containers
- DevOps
- Kubernetes
- Orchestration
title: UserAssignedIdentity
---
