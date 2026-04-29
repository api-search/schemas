---
description: An enabled application within the Cobalt embedded integration platform.
layout: schema
name: Application
properties_list:
- description: Application name.
  name: name
  type: string
- description: Application slug identifier.
  name: slug
  type: string
- description: Application icon URL.
  name: icon
  type: string
- description: Application description.
  name: description
  type: string
- description: Authentication type (e.g., oauth2, api_key).
  name: auth_type
  type: string
- description: Whether the application is connected for the linked account.
  name: connected
  type: boolean
provider_name: Cobalt
provider_slug: cobalt
schema_file: json-schema/application.json
slug: application
source_filename: application.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/cobalt/refs/heads/main/json-schema/application.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Application\",\n  \"description\": \"An enabled application within the Cobalt embedded integration platform.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Application name.\"\n    },\n    \"slug\": {\n      \"type\": \"string\",\n      \"description\": \"Application slug identifier.\"\n    },\n    \"icon\": {\n      \"type\": \"string\",\n      \"description\": \"Application icon URL.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Application description.\"\n    },\n    \"auth_type\": {\n      \"type\": \"string\",\n      \"description\": \"Authentication type (e.g., oauth2, api_key).\"\n    },\n    \"connected\": {\n      \"type\": \"boolean\",\n      \"description\"\
  : \"Whether the application is connected for the linked account.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cobalt/refs/heads/main/json-schema/application.json
tags:
- Automation
- Embedded iPaaS
- Integrations
title: Application
---
