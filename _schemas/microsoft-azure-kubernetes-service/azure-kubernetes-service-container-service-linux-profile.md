---
description: Profile for Linux VMs in the container service cluster.
layout: schema
name: ContainerServiceLinuxProfile
properties_list:
- description: The administrator username to use for Linux VMs.
  name: adminUsername
  type: string
- description: The SSH configuration for Linux-based VMs running on Azure.
  name: ssh
  type: object
provider_name: Azure Kubernetes Service
provider_slug: microsoft-azure-kubernetes-service
schema_file: json-schema/azure-kubernetes-service-container-service-linux-profile-schema.json
slug: azure-kubernetes-service-container-service-linux-profile
source_filename: azure-kubernetes-service-container-service-linux-profile-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ContainerServiceLinuxProfile\",\n  \"type\": \"object\",\n  \"description\": \"Profile for Linux VMs in the container service cluster.\",\n  \"properties\": {\n    \"adminUsername\": {\n      \"type\": \"string\",\n      \"description\": \"The administrator username to use for Linux VMs.\"\n    },\n    \"ssh\": {\n      \"type\": \"object\",\n      \"description\": \"The SSH configuration for Linux-based VMs running on Azure.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-kubernetes-service/refs/heads/main/json-schema/azure-kubernetes-service-container-service-linux-profile-schema.json
tags:
- Azure
- Cloud
- Containers
- DevOps
- Kubernetes
- Orchestration
title: ContainerServiceLinuxProfile
---
