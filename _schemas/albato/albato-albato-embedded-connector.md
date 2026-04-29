---
description: An available app connector for embedded integrations
layout: schema
name: Connector
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: category
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: triggers_count
  type: integer
- description: ''
  name: actions_count
  type: integer
- description: ''
  name: icon_url
  type: string
provider_name: Albato
provider_slug: albato
schema_file: json-schema/albato-albato-embedded-connector-schema.json
slug: albato-albato-embedded-connector
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/albato/refs/heads/main/json-schema/albato-albato-embedded-connector-schema.json\",\n  \"title\": \"Connector\",\n  \"description\": \"An available app connector for embedded integrations\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"category\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"triggers_count\": {\n      \"type\": \"integer\"\n    },\n    \"actions_count\": {\n      \"type\": \"integer\"\n    },\n    \"icon_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/albato/refs/heads/main/json-schema/albato-albato-embedded-connector-schema.json
tags:
- No-Code Automation
- Workflow Automation
- Embedded iPaaS
- App Integration
- Integrations
- Webhooks
- White-Label
title: Connector
---
