---
description: Agent pool resource within a managed cluster.
layout: schema
name: AgentPool
properties_list:
- description: Resource ID.
  name: id
  type: string
- description: The name of the resource that is unique within a resource group.
  name: name
  type: string
- description: Resource type.
  name: type
  type: string
provider_name: Azure Kubernetes Service
provider_slug: azure-kubernetes-service
schema_file: json-schema/azure-kubernetes-service-agent-pool-schema.json
slug: azure-kubernetes-service-agent-pool
source_filename: azure-kubernetes-service-agent-pool-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AgentPool\",\n  \"type\": \"object\",\n  \"description\": \"Agent pool resource within a managed cluster.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Resource ID.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the resource that is unique within a resource group.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Resource type.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-kubernetes-service/refs/heads/main/json-schema/azure-kubernetes-service-agent-pool-schema.json
tags:
- Azure
- Cloud
- Containers
- DevOps
- Kubernetes
- Orchestration
title: AgentPool
---
