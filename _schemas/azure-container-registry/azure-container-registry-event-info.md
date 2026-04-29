---
description: The basic information of an event.
layout: schema
name: EventInfo
properties_list:
- description: The event ID.
  name: id
  type: string
provider_name: Azure Container Registry
provider_slug: azure-container-registry
schema_file: json-schema/azure-container-registry-event-info-schema.json
slug: azure-container-registry-event-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-container-registry/refs/heads/main/json-schema/azure-container-registry-event-info-schema.json\",\n  \"title\": \"EventInfo\",\n  \"description\": \"The basic information of an event.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"description\": \"The event ID.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-container-registry/refs/heads/main/json-schema/azure-container-registry-event-info-schema.json
tags:
- Azure
- Container Images
- Containers
- Docker
- Registry
title: EventInfo
---
