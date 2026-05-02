---
description: Settings for upgrading an agentpool.
layout: schema
name: AgentPoolUpgradeSettings
properties_list:
- description: The maximum number or percentage of nodes that are surged during upgrade. This can either be set to an integer (e.g. 5) or a percentage (e.g. 50%). If a percentage is specified, it is the percentage o
  name: maxSurge
  type: string
- description: The amount of time (in minutes) to wait on eviction of pods and graceful termination per node.
  name: drainTimeoutInMinutes
  type: integer
- description: The amount of time (in minutes) to wait after draining a node and before reimaging it and moving on to the next node.
  name: nodeSoakDurationInMinutes
  type: integer
provider_name: Azure Kubernetes Service
provider_slug: microsoft-azure-kubernetes-service
schema_file: json-schema/azure-kubernetes-service-agent-pool-upgrade-settings-schema.json
slug: azure-kubernetes-service-agent-pool-upgrade-settings
source_filename: azure-kubernetes-service-agent-pool-upgrade-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AgentPoolUpgradeSettings\",\n  \"type\": \"object\",\n  \"description\": \"Settings for upgrading an agentpool.\",\n  \"properties\": {\n    \"maxSurge\": {\n      \"type\": \"string\",\n      \"description\": \"The maximum number or percentage of nodes that are surged during upgrade. This can either be set to an integer (e.g. 5) or a percentage (e.g. 50%). If a percentage is specified, it is the percentage of the total agent pool size at the time of the upgrade.\"\n    },\n    \"drainTimeoutInMinutes\": {\n      \"type\": \"integer\",\n      \"description\": \"The amount of time (in minutes) to wait on eviction of pods and graceful termination per node.\"\n    },\n    \"nodeSoakDurationInMinutes\": {\n      \"type\": \"integer\",\n      \"description\": \"The amount of time (in minutes) to wait after draining a node and before reimaging it and moving on to the next node.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-kubernetes-service/refs/heads/main/json-schema/azure-kubernetes-service-agent-pool-upgrade-settings-schema.json
tags:
- Azure
- Cloud
- Containers
- DevOps
- Kubernetes
- Orchestration
title: AgentPoolUpgradeSettings
---
