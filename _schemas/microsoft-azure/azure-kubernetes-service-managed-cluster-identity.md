---
description: Identity for the managed cluster.
layout: schema
name: ManagedClusterIdentity
properties_list:
- description: The principal ID of the system-assigned identity.
  name: principalId
  type: string
- description: The tenant ID of the system-assigned identity.
  name: tenantId
  type: string
- description: The type of identity used.
  name: type
  type: string
- description: ''
  name: userAssignedIdentities
  type: object
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-kubernetes-service-managed-cluster-identity-schema.json
slug: azure-kubernetes-service-managed-cluster-identity
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ManagedClusterIdentity\",\n  \"type\": \"object\",\n  \"description\": \"Identity for the managed cluster.\",\n  \"properties\": {\n    \"principalId\": {\n      \"type\": \"string\",\n      \"description\": \"The principal ID of the system-assigned identity.\"\n    },\n    \"tenantId\": {\n      \"type\": \"string\",\n      \"description\": \"The tenant ID of the system-assigned identity.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of identity used.\"\n    },\n    \"userAssignedIdentities\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-kubernetes-service-managed-cluster-identity-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: ManagedClusterIdentity
---
