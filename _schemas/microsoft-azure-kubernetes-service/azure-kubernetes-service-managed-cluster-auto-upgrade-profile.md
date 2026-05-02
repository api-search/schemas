---
description: Auto upgrade profile for a managed cluster.
layout: schema
name: ManagedClusterAutoUpgradeProfile
properties_list:
- description: The upgrade channel for auto upgrade.
  name: upgradeChannel
  type: string
- description: The node OS upgrade channel. Manner in which the OS on your nodes is updated.
  name: nodeOSUpgradeChannel
  type: string
provider_name: Azure Kubernetes Service
provider_slug: microsoft-azure-kubernetes-service
schema_file: json-schema/azure-kubernetes-service-managed-cluster-auto-upgrade-profile-schema.json
slug: azure-kubernetes-service-managed-cluster-auto-upgrade-profile
source_filename: azure-kubernetes-service-managed-cluster-auto-upgrade-profile-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ManagedClusterAutoUpgradeProfile\",\n  \"type\": \"object\",\n  \"description\": \"Auto upgrade profile for a managed cluster.\",\n  \"properties\": {\n    \"upgradeChannel\": {\n      \"type\": \"string\",\n      \"description\": \"The upgrade channel for auto upgrade.\"\n    },\n    \"nodeOSUpgradeChannel\": {\n      \"type\": \"string\",\n      \"description\": \"The node OS upgrade channel. Manner in which the OS on your nodes is updated.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-kubernetes-service/refs/heads/main/json-schema/azure-kubernetes-service-managed-cluster-auto-upgrade-profile-schema.json
tags:
- Azure
- Cloud
- Containers
- DevOps
- Kubernetes
- Orchestration
title: ManagedClusterAutoUpgradeProfile
---
