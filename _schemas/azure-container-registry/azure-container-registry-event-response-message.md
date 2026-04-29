---
description: The event response message received from the service URI.
layout: schema
name: EventResponseMessage
properties_list:
- description: The content of the event response message.
  name: content
  type: string
- description: The headers of the event response message.
  name: headers
  type: object
- description: The reason phrase of the event response message.
  name: reasonPhrase
  type: string
- description: The status code of the event response message.
  name: statusCode
  type: string
- description: The HTTP message version.
  name: version
  type: string
provider_name: Azure Container Registry
provider_slug: azure-container-registry
schema_file: json-schema/azure-container-registry-event-response-message-schema.json
slug: azure-container-registry-event-response-message
source_filename: azure-container-registry-event-response-message-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-container-registry/refs/heads/main/json-schema/azure-container-registry-event-response-message-schema.json\",\n  \"title\": \"EventResponseMessage\",\n  \"description\": \"The event response message received from the service URI.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"content\": {\n      \"description\": \"The content of the event response message.\",\n      \"type\": \"string\"\n    },\n    \"headers\": {\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"The headers of the event response message.\",\n      \"type\": \"object\"\n    },\n    \"reasonPhrase\": {\n      \"description\": \"The reason phrase of the event response message.\",\n      \"type\": \"string\"\n    },\n    \"statusCode\": {\n      \"description\": \"The status code of the event response message.\",\n \
  \     \"type\": \"string\"\n    },\n    \"version\": {\n      \"description\": \"The HTTP message version.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-container-registry/refs/heads/main/json-schema/azure-container-registry-event-response-message-schema.json
tags:
- Azure
- Container Images
- Containers
- Docker
- Registry
title: EventResponseMessage
---
