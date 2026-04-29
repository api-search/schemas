---
description: The event request message sent to the service URI.
layout: schema
name: EventRequestMessage
properties_list:
- description: The content of the event request message.
  name: content
  type: object
- description: The headers of the event request message.
  name: headers
  type: object
- description: The HTTP method used to send the event request message.
  name: method
  type: string
- description: The URI used to send the event request message.
  name: requestUri
  type: string
- description: The HTTP message version.
  name: version
  type: string
provider_name: Azure Container Registry
provider_slug: azure-container-registry
schema_file: json-schema/azure-container-registry-event-request-message-schema.json
slug: azure-container-registry-event-request-message
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-container-registry/refs/heads/main/json-schema/azure-container-registry-event-request-message-schema.json\",\n  \"title\": \"EventRequestMessage\",\n  \"description\": \"The event request message sent to the service URI.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"content\": {\n      \"$ref\": \"#/definitions/EventContent\",\n      \"description\": \"The content of the event request message.\"\n    },\n    \"headers\": {\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"The headers of the event request message.\",\n      \"type\": \"object\"\n    },\n    \"method\": {\n      \"description\": \"The HTTP method used to send the event request message.\",\n      \"type\": \"string\"\n    },\n    \"requestUri\": {\n      \"description\": \"The URI used to send the event request message.\"\
  ,\n      \"type\": \"string\"\n    },\n    \"version\": {\n      \"description\": \"The HTTP message version.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-container-registry/refs/heads/main/json-schema/azure-container-registry-event-request-message-schema.json
tags:
- Azure
- Container Images
- Containers
- Docker
- Registry
title: EventRequestMessage
---
