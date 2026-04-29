---
description: Input schema for creating or updating a Plugin.
layout: schema
name: PluginInput
properties_list:
- description: The name of the plugin.
  name: name
  type: string
- description: ''
  name: instance_name
  type: string
- description: ''
  name: config
  type: object
- description: ''
  name: protocols
  type: array
- description: ''
  name: enabled
  type: boolean
- description: ''
  name: tags
  type: array
- description: ''
  name: ordering
  type: object
- description: ''
  name: service
  type: object
- description: ''
  name: route
  type: object
- description: ''
  name: consumer
  type: object
- description: ''
  name: consumer_group
  type: object
provider_name: Kong
provider_slug: kong
schema_file: json-schema/kong-gateway-admin-plugin-input-schema.json
slug: kong-gateway-admin-plugin-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PluginInput\",\n  \"type\": \"object\",\n  \"description\": \"Input schema for creating or updating a Plugin.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the plugin.\"\n    },\n    \"instance_name\": {\n      \"type\": \"string\"\n    },\n    \"config\": {\n      \"type\": \"object\"\n    },\n    \"protocols\": {\n      \"type\": \"array\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\"\n    },\n    \"tags\": {\n      \"type\": \"array\"\n    },\n    \"ordering\": {\n      \"type\": \"object\"\n    },\n    \"service\": {\n      \"type\": \"object\"\n    },\n    \"route\": {\n      \"type\": \"object\"\n    },\n    \"consumer\": {\n      \"type\": \"object\"\n    },\n    \"consumer_group\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/kong/refs/heads/main/json-schema/kong-gateway-admin-plugin-input-schema.json
tags:
- API Gateway
- Lua
- NGINX
- Open Source
title: PluginInput
---
