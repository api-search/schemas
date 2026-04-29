---
description: The agent that initiated the event. For most situations, this could be from the authorization context of the request.
layout: schema
name: Actor
properties_list:
- description: The subject or username associated with the request context that generated the event.
  name: name
  type: string
provider_name: Azure Container Registry
provider_slug: azure-container-registry
schema_file: json-schema/azure-container-registry-actor-schema.json
slug: azure-container-registry-actor
source_filename: azure-container-registry-actor-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-container-registry/refs/heads/main/json-schema/azure-container-registry-actor-schema.json\",\n  \"title\": \"Actor\",\n  \"description\": \"The agent that initiated the event. For most situations, this could be from the authorization context of the request.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"description\": \"The subject or username associated with the request context that generated the event.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-container-registry/refs/heads/main/json-schema/azure-container-registry-actor-schema.json
tags:
- Azure
- Container Images
- Containers
- Docker
- Registry
title: Actor
---
