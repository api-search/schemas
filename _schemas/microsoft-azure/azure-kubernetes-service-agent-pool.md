---
description: Agent pool resource.
layout: schema
name: AgentPool
properties_list:
- description: Resource ID.
  name: id
  type: string
- description: Resource name.
  name: name
  type: string
- description: Resource type.
  name: type
  type: string
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-kubernetes-service-agent-pool-schema.json
slug: azure-kubernetes-service-agent-pool
source_filename: azure-kubernetes-service-agent-pool-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AgentPool\",\n  \"type\": \"object\",\n  \"description\": \"Agent pool resource.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Resource ID.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Resource name.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Resource type.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-kubernetes-service-agent-pool-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: AgentPool
---
