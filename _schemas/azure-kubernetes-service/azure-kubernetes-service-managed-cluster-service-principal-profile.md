---
description: Information about a service principal identity for the cluster to use for manipulating Azure APIs.
layout: schema
name: ManagedClusterServicePrincipalProfile
properties_list:
- description: The ID for the service principal.
  name: clientId
  type: string
- description: The secret password associated with the service principal.
  name: secret
  type: string
provider_name: Azure Kubernetes Service
provider_slug: azure-kubernetes-service
schema_file: json-schema/azure-kubernetes-service-managed-cluster-service-principal-profile-schema.json
slug: azure-kubernetes-service-managed-cluster-service-principal-profile
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ManagedClusterServicePrincipalProfile\",\n  \"type\": \"object\",\n  \"description\": \"Information about a service principal identity for the cluster to use for manipulating Azure APIs.\",\n  \"properties\": {\n    \"clientId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID for the service principal.\"\n    },\n    \"secret\": {\n      \"type\": \"string\",\n      \"description\": \"The secret password associated with the service principal.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-kubernetes-service/refs/heads/main/json-schema/azure-kubernetes-service-managed-cluster-service-principal-profile-schema.json
tags:
- Azure
- Cloud
- Containers
- DevOps
- Kubernetes
- Orchestration
title: ManagedClusterServicePrincipalProfile
---
