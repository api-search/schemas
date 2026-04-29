---
description: Identity for the managed cluster.
layout: schema
name: ManagedClusterIdentity
properties_list:
- description: The principal id of the system assigned identity associated with this resource.
  name: principalId
  type: string
- description: The tenant id of the system assigned identity associated with this resource.
  name: tenantId
  type: string
- description: The type of identity used for the managed cluster.
  name: type
  type: string
- description: The keys must be ARM resource IDs in the form of /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ManagedIdentity/userAssignedIdentities/{identityName}.
  name: userAssignedIdentities
  type: object
provider_name: Azure Kubernetes Service
provider_slug: azure-kubernetes-service
schema_file: json-schema/azure-kubernetes-service-managed-cluster-identity-schema.json
slug: azure-kubernetes-service-managed-cluster-identity
source_filename: azure-kubernetes-service-managed-cluster-identity-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ManagedClusterIdentity\",\n  \"type\": \"object\",\n  \"description\": \"Identity for the managed cluster.\",\n  \"properties\": {\n    \"principalId\": {\n      \"type\": \"string\",\n      \"description\": \"The principal id of the system assigned identity associated with this resource.\"\n    },\n    \"tenantId\": {\n      \"type\": \"string\",\n      \"description\": \"The tenant id of the system assigned identity associated with this resource.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of identity used for the managed cluster.\"\n    },\n    \"userAssignedIdentities\": {\n      \"type\": \"object\",\n      \"description\": \"The keys must be ARM resource IDs in the form of /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ManagedIdentity/userAssignedIdentities/{identityName}.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-kubernetes-service/refs/heads/main/json-schema/azure-kubernetes-service-managed-cluster-identity-schema.json
tags:
- Azure
- Cloud
- Containers
- DevOps
- Kubernetes
- Orchestration
title: ManagedClusterIdentity
---
