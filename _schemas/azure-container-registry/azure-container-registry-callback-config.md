---
description: The configuration of service URI and custom headers for the webhook.
layout: schema
name: CallbackConfig
properties_list:
- description: Custom headers that will be added to the webhook notifications.
  name: customHeaders
  type: object
- description: The service URI for the webhook to post notifications.
  name: serviceUri
  type: string
provider_name: Azure Container Registry
provider_slug: azure-container-registry
schema_file: json-schema/azure-container-registry-callback-config-schema.json
slug: azure-container-registry-callback-config
source_filename: azure-container-registry-callback-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-container-registry/refs/heads/main/json-schema/azure-container-registry-callback-config-schema.json\",\n  \"title\": \"CallbackConfig\",\n  \"description\": \"The configuration of service URI and custom headers for the webhook.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"customHeaders\": {\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Custom headers that will be added to the webhook notifications.\",\n      \"type\": \"object\"\n    },\n    \"serviceUri\": {\n      \"description\": \"The service URI for the webhook to post notifications.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"serviceUri\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-container-registry/refs/heads/main/json-schema/azure-container-registry-callback-config-schema.json
tags:
- Azure
- Container Images
- Containers
- Docker
- Registry
title: CallbackConfig
---
