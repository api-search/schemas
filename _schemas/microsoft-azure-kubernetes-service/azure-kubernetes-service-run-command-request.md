---
description: A run command request.
layout: schema
name: RunCommandRequest
properties_list:
- description: The command to run.
  name: command
  type: string
- description: A base64 encoded zip file containing the files required by the command.
  name: context
  type: string
- description: AuthToken issued for AKS AAD Server App.
  name: clusterToken
  type: string
provider_name: Azure Kubernetes Service
provider_slug: microsoft-azure-kubernetes-service
schema_file: json-schema/azure-kubernetes-service-run-command-request-schema.json
slug: azure-kubernetes-service-run-command-request
source_filename: azure-kubernetes-service-run-command-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RunCommandRequest\",\n  \"type\": \"object\",\n  \"description\": \"A run command request.\",\n  \"properties\": {\n    \"command\": {\n      \"type\": \"string\",\n      \"description\": \"The command to run.\"\n    },\n    \"context\": {\n      \"type\": \"string\",\n      \"description\": \"A base64 encoded zip file containing the files required by the command.\"\n    },\n    \"clusterToken\": {\n      \"type\": \"string\",\n      \"description\": \"AuthToken issued for AKS AAD Server App.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-kubernetes-service/refs/heads/main/json-schema/azure-kubernetes-service-run-command-request-schema.json
tags:
- Azure
- Cloud
- Containers
- DevOps
- Kubernetes
- Orchestration
title: RunCommandRequest
---
