---
description: Result of a configuration reload operation.
layout: schema
name: ReloadResponse
properties_list:
- description: Whether the reload succeeded.
  name: success
  type: boolean
- description: Human-readable result message.
  name: message
  type: string
- description: Name of the reloaded configuration.
  name: name
  type: string
provider_name: BFE
provider_slug: bfe
schema_file: json-schema/bfe-reload-response-schema.json
slug: bfe-reload-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bfe/refs/heads/main/json-schema/bfe-reload-response-schema.json\",\n  \"title\": \"ReloadResponse\",\n  \"description\": \"Result of a configuration reload operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"success\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the reload succeeded.\",\n      \"example\": true\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable result message.\",\n      \"example\": \"Configuration reloaded successfully\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the reloaded configuration.\",\n      \"example\": \"server_data_conf\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bfe/refs/heads/main/json-schema/bfe-reload-response-schema.json
tags:
- Load Balancer
- Networking
- Open Source
- Traffic Management
- CNCF
- Baidu
title: ReloadResponse
---
