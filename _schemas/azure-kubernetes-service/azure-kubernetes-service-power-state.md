---
description: Describes the Power State of the cluster.
layout: schema
name: PowerState
properties_list:
- description: Tells whether the cluster is Running or Stopped.
  name: code
  type: string
provider_name: Azure Kubernetes Service
provider_slug: azure-kubernetes-service
schema_file: json-schema/azure-kubernetes-service-power-state-schema.json
slug: azure-kubernetes-service-power-state
source_filename: azure-kubernetes-service-power-state-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PowerState\",\n  \"type\": \"object\",\n  \"description\": \"Describes the Power State of the cluster.\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"Tells whether the cluster is Running or Stopped.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-kubernetes-service/refs/heads/main/json-schema/azure-kubernetes-service-power-state-schema.json
tags:
- Azure
- Cloud
- Containers
- DevOps
- Kubernetes
- Orchestration
title: PowerState
---
