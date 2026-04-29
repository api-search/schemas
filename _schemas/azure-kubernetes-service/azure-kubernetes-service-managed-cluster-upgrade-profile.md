---
description: The list of available upgrades for compute pools.
layout: schema
name: ManagedClusterUpgradeProfile
properties_list:
- description: The ID of the upgrade profile.
  name: id
  type: string
- description: The name of the upgrade profile.
  name: name
  type: string
- description: The type of the upgrade profile.
  name: type
  type: string
- description: ''
  name: properties
  type: object
provider_name: Azure Kubernetes Service
provider_slug: azure-kubernetes-service
schema_file: json-schema/azure-kubernetes-service-managed-cluster-upgrade-profile-schema.json
slug: azure-kubernetes-service-managed-cluster-upgrade-profile
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ManagedClusterUpgradeProfile\",\n  \"type\": \"object\",\n  \"description\": \"The list of available upgrades for compute pools.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the upgrade profile.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the upgrade profile.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the upgrade profile.\"\n    },\n    \"properties\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-kubernetes-service/refs/heads/main/json-schema/azure-kubernetes-service-managed-cluster-upgrade-profile-schema.json
tags:
- Azure
- Cloud
- Containers
- DevOps
- Kubernetes
- Orchestration
title: ManagedClusterUpgradeProfile
---
