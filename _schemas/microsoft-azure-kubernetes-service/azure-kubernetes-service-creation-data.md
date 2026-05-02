---
description: Data used when creating a target resource from a source resource.
layout: schema
name: CreationData
properties_list:
- description: This is the ARM ID of the source object to be used to create the target object.
  name: sourceResourceId
  type: string
provider_name: Azure Kubernetes Service
provider_slug: microsoft-azure-kubernetes-service
schema_file: json-schema/azure-kubernetes-service-creation-data-schema.json
slug: azure-kubernetes-service-creation-data
source_filename: azure-kubernetes-service-creation-data-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreationData\",\n  \"type\": \"object\",\n  \"description\": \"Data used when creating a target resource from a source resource.\",\n  \"properties\": {\n    \"sourceResourceId\": {\n      \"type\": \"string\",\n      \"description\": \"This is the ARM ID of the source object to be used to create the target object.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-kubernetes-service/refs/heads/main/json-schema/azure-kubernetes-service-creation-data-schema.json
tags:
- Azure
- Cloud
- Containers
- DevOps
- Kubernetes
- Orchestration
title: CreationData
---
