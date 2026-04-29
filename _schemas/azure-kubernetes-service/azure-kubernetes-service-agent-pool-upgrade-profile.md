---
description: The list of available upgrades for an agent pool.
layout: schema
name: AgentPoolUpgradeProfile
properties_list:
- description: The ID of the agent pool upgrade profile.
  name: id
  type: string
- description: The name of the agent pool upgrade profile.
  name: name
  type: string
- description: The type of the agent pool upgrade profile.
  name: type
  type: string
- description: ''
  name: properties
  type: object
provider_name: Azure Kubernetes Service
provider_slug: azure-kubernetes-service
schema_file: json-schema/azure-kubernetes-service-agent-pool-upgrade-profile-schema.json
slug: azure-kubernetes-service-agent-pool-upgrade-profile
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AgentPoolUpgradeProfile\",\n  \"type\": \"object\",\n  \"description\": \"The list of available upgrades for an agent pool.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the agent pool upgrade profile.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the agent pool upgrade profile.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the agent pool upgrade profile.\"\n    },\n    \"properties\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-kubernetes-service/refs/heads/main/json-schema/azure-kubernetes-service-agent-pool-upgrade-profile-schema.json
tags:
- Azure
- Cloud
- Containers
- DevOps
- Kubernetes
- Orchestration
title: AgentPoolUpgradeProfile
---
