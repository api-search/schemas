---
description: The event for a webhook.
layout: schema
name: Event
properties_list:
- description: The event request message sent to the service URI.
  name: eventRequestMessage
  type: object
- description: The event response message received from the service URI.
  name: eventResponseMessage
  type: object
provider_name: Azure Container Registry
provider_slug: azure-container-registry
schema_file: json-schema/azure-container-registry-event-schema.json
slug: azure-container-registry-event
source_filename: azure-container-registry-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-container-registry/refs/heads/main/json-schema/azure-container-registry-event-schema.json\",\n  \"title\": \"Event\",\n  \"description\": \"The event for a webhook.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"eventRequestMessage\": {\n      \"$ref\": \"#/definitions/EventRequestMessage\",\n      \"description\": \"The event request message sent to the service URI.\"\n    },\n    \"eventResponseMessage\": {\n      \"$ref\": \"#/definitions/EventResponseMessage\",\n      \"description\": \"The event response message received from the service URI.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-container-registry/refs/heads/main/json-schema/azure-container-registry-event-schema.json
tags:
- Azure
- Container Images
- Containers
- Docker
- Registry
title: Event
---
