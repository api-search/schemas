---
description: The container exec request.
layout: schema
name: ContainerExecRequest
properties_list:
- description: The command to be executed.
  name: command
  type: string
- description: The size of the terminal.
  name: terminalSize
  type: object
provider_name: Azure Container Instances
provider_slug: azure-container-instances
schema_file: json-schema/azure-container-instances-container-exec-request-schema.json
slug: azure-container-instances-container-exec-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-container-instances/refs/heads/main/json-schema/azure-container-instances-container-exec-request-schema.json\",\n  \"title\": \"ContainerExecRequest\",\n  \"description\": \"The container exec request.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"command\": {\n      \"description\": \"The command to be executed.\",\n      \"type\": \"string\"\n    },\n    \"terminalSize\": {\n      \"description\": \"The size of the terminal.\",\n      \"properties\": {\n        \"cols\": {\n          \"description\": \"The column size of the terminal\",\n          \"type\": \"integer\"\n        },\n        \"rows\": {\n          \"description\": \"The row size of the terminal\",\n          \"type\": \"integer\"\n        }\n      },\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-container-instances/refs/heads/main/json-schema/azure-container-instances-container-exec-request-schema.json
tags:
- Azure
- Cloud
- Container Instances
- Containers
- Microsoft
- Serverless
title: ContainerExecRequest
---
