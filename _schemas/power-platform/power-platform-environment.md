---
description: A Power Platform environment resource. Environments are containers that store apps, flows, data, and other resources.
layout: schema
name: Environment
properties_list:
- description: The fully qualified resource ID of the environment.
  name: id
  type: string
- description: The resource type.
  name: type
  type: string
- description: The geographic location of the environment.
  name: location
  type: string
- description: The environment identifier (GUID).
  name: name
  type: string
provider_name: Microsoft Power Platform APIs
provider_slug: power-platform
schema_file: json-schema/power-platform-environment-schema.json
slug: power-platform-environment
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Environment\",\n  \"type\": \"object\",\n  \"description\": \"A Power Platform environment resource. Environments are containers that store apps, flows, data, and other resources.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The fully qualified resource ID of the environment.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The resource type.\"\n    },\n    \"location\": {\n      \"type\": \"string\",\n      \"description\": \"The geographic location of the environment.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The environment identifier (GUID).\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/power-platform/refs/heads/main/json-schema/power-platform-environment-schema.json
tags:
- Business Applications
- Copilot Studio
- Dataverse
- Low-Code
- Microsoft
- No-Code
- Power Pages
- Power Platform
title: Environment
---
