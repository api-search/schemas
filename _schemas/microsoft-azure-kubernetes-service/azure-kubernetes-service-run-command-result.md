---
description: Run command result.
layout: schema
name: RunCommandResult
properties_list:
- description: The command id.
  name: id
  type: string
- description: ''
  name: properties
  type: object
provider_name: Azure Kubernetes Service
provider_slug: microsoft-azure-kubernetes-service
schema_file: json-schema/azure-kubernetes-service-run-command-result-schema.json
slug: azure-kubernetes-service-run-command-result
source_filename: azure-kubernetes-service-run-command-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RunCommandResult\",\n  \"type\": \"object\",\n  \"description\": \"Run command result.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The command id.\"\n    },\n    \"properties\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-kubernetes-service/refs/heads/main/json-schema/azure-kubernetes-service-run-command-result-schema.json
tags:
- Azure
- Cloud
- Containers
- DevOps
- Kubernetes
- Orchestration
title: RunCommandResult
---
