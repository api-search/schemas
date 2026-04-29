---
description: The information for the container exec command.
layout: schema
name: ContainerExecResponse
properties_list:
- description: The password to start the exec command.
  name: password
  type: string
- description: The uri for the exec websocket.
  name: webSocketUri
  type: string
provider_name: Azure Container Instances
provider_slug: azure-container-instances
schema_file: json-schema/azure-container-instances-container-exec-response-schema.json
slug: azure-container-instances-container-exec-response
source_filename: azure-container-instances-container-exec-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-container-instances/refs/heads/main/json-schema/azure-container-instances-container-exec-response-schema.json\",\n  \"title\": \"ContainerExecResponse\",\n  \"description\": \"The information for the container exec command.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"password\": {\n      \"description\": \"The password to start the exec command.\",\n      \"type\": \"string\"\n    },\n    \"webSocketUri\": {\n      \"description\": \"The uri for the exec websocket.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-container-instances/refs/heads/main/json-schema/azure-container-instances-container-exec-response-schema.json
tags:
- Azure
- Cloud
- Container Instances
- Containers
- Microsoft
- Serverless
title: ContainerExecResponse
---
