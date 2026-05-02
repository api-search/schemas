---
description: A Kubernetes add-on profile for a managed cluster.
layout: schema
name: ManagedClusterAddonProfile
properties_list:
- description: Whether the add-on is enabled or not.
  name: enabled
  type: boolean
- description: Key-value pairs for configuring an add-on.
  name: config
  type: object
provider_name: Azure Kubernetes Service
provider_slug: microsoft-azure-kubernetes-service
schema_file: json-schema/azure-kubernetes-service-managed-cluster-addon-profile-schema.json
slug: azure-kubernetes-service-managed-cluster-addon-profile
source_filename: azure-kubernetes-service-managed-cluster-addon-profile-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ManagedClusterAddonProfile\",\n  \"type\": \"object\",\n  \"description\": \"A Kubernetes add-on profile for a managed cluster.\",\n  \"properties\": {\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the add-on is enabled or not.\"\n    },\n    \"config\": {\n      \"type\": \"object\",\n      \"description\": \"Key-value pairs for configuring an add-on.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-kubernetes-service/refs/heads/main/json-schema/azure-kubernetes-service-managed-cluster-addon-profile-schema.json
tags:
- Azure
- Cloud
- Containers
- DevOps
- Kubernetes
- Orchestration
title: ManagedClusterAddonProfile
---
