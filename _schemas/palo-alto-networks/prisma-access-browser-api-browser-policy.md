---
description: BrowserPolicy schema from Palo Alto Networks Prisma Access Browser Management API
layout: schema
name: BrowserPolicy
properties_list:
- description: Unique identifier of the browser policy.
  name: policy_id
  type: string
- description: Display name of the policy.
  name: name
  type: string
- description: Description of the policy's purpose.
  name: description
  type: string
- description: Whether the policy is active.
  name: enabled
  type: boolean
- description: Web filtering configuration.
  name: web_filtering
  type: object
- description: Whether DLP controls are enabled.
  name: dlp_enabled
  type: boolean
- description: Extension installation policy.
  name: extension_policy
  type: string
- description: File download control setting.
  name: download_control
  type: string
- description: ''
  name: created_at
  type: string
- description: ''
  name: updated_at
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-access-browser-api-browser-policy-schema.json
slug: prisma-access-browser-api-browser-policy
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BrowserPolicy\",\n  \"description\": \"BrowserPolicy schema from Palo Alto Networks Prisma Access Browser Management API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-access-browser-api-browser-policy-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"policy_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the browser policy.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the policy.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the policy's purpose.\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the policy is active.\"\n    },\n    \"web_filtering\": {\n      \"type\": \"object\",\n      \"description\": \"Web filtering\
  \ configuration.\",\n      \"properties\": {\n        \"enabled\": {\n          \"type\": \"boolean\"\n        },\n        \"blocked_categories\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"dlp_enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether DLP controls are enabled.\"\n    },\n    \"extension_policy\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"allow_all\",\n        \"allow_list\",\n        \"block_all\"\n      ],\n      \"description\": \"Extension installation policy.\"\n    },\n    \"download_control\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"allow\",\n        \"scan\",\n        \"block\"\n      ],\n      \"description\": \"File download control setting.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\"\
  : \"date-time\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-access-browser-api-browser-policy-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: BrowserPolicy
---
