---
description: Metadata pertaining to creation and last modification of the resource.
layout: schema
name: SystemData
properties_list:
- description: The identity that created the resource.
  name: createdBy
  type: string
- description: The type of identity that created the resource.
  name: createdByType
  type: string
- description: The timestamp of resource creation (UTC).
  name: createdAt
  type: string
- description: The identity that last modified the resource.
  name: lastModifiedBy
  type: string
- description: The type of identity that last modified the resource.
  name: lastModifiedByType
  type: string
- description: The timestamp of resource last modification (UTC).
  name: lastModifiedAt
  type: string
provider_name: Azure Kubernetes Service
provider_slug: azure-kubernetes-service
schema_file: json-schema/azure-kubernetes-service-system-data-schema.json
slug: azure-kubernetes-service-system-data
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SystemData\",\n  \"type\": \"object\",\n  \"description\": \"Metadata pertaining to creation and last modification of the resource.\",\n  \"properties\": {\n    \"createdBy\": {\n      \"type\": \"string\",\n      \"description\": \"The identity that created the resource.\"\n    },\n    \"createdByType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of identity that created the resource.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"description\": \"The timestamp of resource creation (UTC).\"\n    },\n    \"lastModifiedBy\": {\n      \"type\": \"string\",\n      \"description\": \"The identity that last modified the resource.\"\n    },\n    \"lastModifiedByType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of identity that last modified the resource.\"\n    },\n    \"lastModifiedAt\": {\n      \"type\": \"string\",\n      \"\
  description\": \"The timestamp of resource last modification (UTC).\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-kubernetes-service/refs/heads/main/json-schema/azure-kubernetes-service-system-data-schema.json
tags:
- Azure
- Cloud
- Containers
- DevOps
- Kubernetes
- Orchestration
title: SystemData
---
