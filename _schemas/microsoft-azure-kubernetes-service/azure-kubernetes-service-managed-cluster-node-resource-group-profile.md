---
description: Node resource group lockdown profile for a managed cluster.
layout: schema
name: ManagedClusterNodeResourceGroupProfile
properties_list:
- description: The restriction level applied to the cluster node resource group.
  name: restrictionLevel
  type: string
provider_name: Azure Kubernetes Service
provider_slug: microsoft-azure-kubernetes-service
schema_file: json-schema/azure-kubernetes-service-managed-cluster-node-resource-group-profile-schema.json
slug: azure-kubernetes-service-managed-cluster-node-resource-group-profile
source_filename: azure-kubernetes-service-managed-cluster-node-resource-group-profile-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ManagedClusterNodeResourceGroupProfile\",\n  \"type\": \"object\",\n  \"description\": \"Node resource group lockdown profile for a managed cluster.\",\n  \"properties\": {\n    \"restrictionLevel\": {\n      \"type\": \"string\",\n      \"description\": \"The restriction level applied to the cluster node resource group.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-kubernetes-service/refs/heads/main/json-schema/azure-kubernetes-service-managed-cluster-node-resource-group-profile-schema.json
tags:
- Azure
- Cloud
- Containers
- DevOps
- Kubernetes
- Orchestration
title: ManagedClusterNodeResourceGroupProfile
---
