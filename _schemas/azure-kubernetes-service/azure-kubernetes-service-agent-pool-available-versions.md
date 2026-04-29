---
description: The available agent pool versions.
layout: schema
name: AgentPoolAvailableVersions
properties_list:
- description: The ID of the agent pool version list.
  name: id
  type: string
- description: The name of the agent pool version list.
  name: name
  type: string
- description: The resource type.
  name: type
  type: string
- description: ''
  name: properties
  type: object
provider_name: Azure Kubernetes Service
provider_slug: azure-kubernetes-service
schema_file: json-schema/azure-kubernetes-service-agent-pool-available-versions-schema.json
slug: azure-kubernetes-service-agent-pool-available-versions
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AgentPoolAvailableVersions\",\n  \"type\": \"object\",\n  \"description\": \"The available agent pool versions.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the agent pool version list.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the agent pool version list.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The resource type.\"\n    },\n    \"properties\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-kubernetes-service/refs/heads/main/json-schema/azure-kubernetes-service-agent-pool-available-versions-schema.json
tags:
- Azure
- Cloud
- Containers
- DevOps
- Kubernetes
- Orchestration
title: AgentPoolAvailableVersions
---
