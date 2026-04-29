---
description: The content of the event request message.
layout: schema
name: EventContent
properties_list:
- description: The action that encompasses the provided event.
  name: action
  type: string
- description: The agent that initiated the event. For most situations, this could be from the authorization context of the request.
  name: actor
  type: object
- description: The event ID.
  name: id
  type: string
- description: The request that generated the event.
  name: request
  type: object
- description: The registry node that generated the event. Put differently, while the actor initiates the event, the source generates it.
  name: source
  type: object
- description: The target of the event.
  name: target
  type: object
- description: The time at which the event occurred.
  name: timestamp
  type: string
provider_name: Azure Container Registry
provider_slug: azure-container-registry
schema_file: json-schema/azure-container-registry-event-content-schema.json
slug: azure-container-registry-event-content
source_filename: azure-container-registry-event-content-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-container-registry/refs/heads/main/json-schema/azure-container-registry-event-content-schema.json\",\n  \"title\": \"EventContent\",\n  \"description\": \"The content of the event request message.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"action\": {\n      \"description\": \"The action that encompasses the provided event.\",\n      \"type\": \"string\"\n    },\n    \"actor\": {\n      \"$ref\": \"#/definitions/Actor\",\n      \"description\": \"The agent that initiated the event. For most situations, this could be from the authorization context of the request.\"\n    },\n    \"id\": {\n      \"description\": \"The event ID.\",\n      \"type\": \"string\"\n    },\n    \"request\": {\n      \"$ref\": \"#/definitions/Request\",\n      \"description\": \"The request that generated the event.\"\n    },\n    \"source\": {\n      \"\
  $ref\": \"#/definitions/Source\",\n      \"description\": \"The registry node that generated the event. Put differently, while the actor initiates the event, the source generates it.\"\n    },\n    \"target\": {\n      \"$ref\": \"#/definitions/Target\",\n      \"description\": \"The target of the event.\"\n    },\n    \"timestamp\": {\n      \"description\": \"The time at which the event occurred.\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-container-registry/refs/heads/main/json-schema/azure-container-registry-event-content-schema.json
tags:
- Azure
- Container Images
- Containers
- Docker
- Registry
title: EventContent
---
