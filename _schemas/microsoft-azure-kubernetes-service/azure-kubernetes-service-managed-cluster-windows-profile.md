---
description: Profile for Windows VMs in the managed cluster.
layout: schema
name: ManagedClusterWindowsProfile
properties_list:
- description: The administrator username to use for Windows VMs.
  name: adminUsername
  type: string
- description: The administrator password to use for Windows VMs.
  name: adminPassword
  type: string
- description: The license type to use for Windows VMs.
  name: licenseType
  type: string
- description: Whether to enable CSI proxy.
  name: enableCSIProxy
  type: boolean
provider_name: Azure Kubernetes Service
provider_slug: microsoft-azure-kubernetes-service
schema_file: json-schema/azure-kubernetes-service-managed-cluster-windows-profile-schema.json
slug: azure-kubernetes-service-managed-cluster-windows-profile
source_filename: azure-kubernetes-service-managed-cluster-windows-profile-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ManagedClusterWindowsProfile\",\n  \"type\": \"object\",\n  \"description\": \"Profile for Windows VMs in the managed cluster.\",\n  \"properties\": {\n    \"adminUsername\": {\n      \"type\": \"string\",\n      \"description\": \"The administrator username to use for Windows VMs.\"\n    },\n    \"adminPassword\": {\n      \"type\": \"string\",\n      \"description\": \"The administrator password to use for Windows VMs.\"\n    },\n    \"licenseType\": {\n      \"type\": \"string\",\n      \"description\": \"The license type to use for Windows VMs.\"\n    },\n    \"enableCSIProxy\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to enable CSI proxy.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-kubernetes-service/refs/heads/main/json-schema/azure-kubernetes-service-managed-cluster-windows-profile-schema.json
tags:
- Azure
- Cloud
- Containers
- DevOps
- Kubernetes
- Orchestration
title: ManagedClusterWindowsProfile
---
