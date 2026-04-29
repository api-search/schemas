---
description: BrowserPolicyRequest schema from Palo Alto Networks Prisma Access Browser Management API
layout: schema
name: BrowserPolicyRequest
properties_list:
- description: Display name for the browser policy.
  name: name
  type: string
- description: Optional description.
  name: description
  type: string
- description: ''
  name: enabled
  type: boolean
- description: ''
  name: web_filtering
  type: object
- description: ''
  name: dlp_enabled
  type: boolean
- description: ''
  name: extension_policy
  type: string
- description: ''
  name: download_control
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-access-browser-api-browser-policy-request-schema.json
slug: prisma-access-browser-api-browser-policy-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BrowserPolicyRequest\",\n  \"description\": \"BrowserPolicyRequest schema from Palo Alto Networks Prisma Access Browser Management API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-access-browser-api-browser-policy-request-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name for the browser policy.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Optional description.\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"default\": true\n    },\n    \"web_filtering\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"enabled\": {\n          \"type\": \"boolean\"\n        },\n        \"blocked_categories\": {\n          \"type\": \"array\",\n          \"items\"\
  : {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"dlp_enabled\": {\n      \"type\": \"boolean\",\n      \"default\": false\n    },\n    \"extension_policy\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"allow_all\",\n        \"allow_list\",\n        \"block_all\"\n      ],\n      \"default\": \"allow_all\"\n    },\n    \"download_control\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"allow\",\n        \"scan\",\n        \"block\"\n      ],\n      \"default\": \"allow\"\n    }\n  },\n  \"required\": [\n    \"name\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-access-browser-api-browser-policy-request-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: BrowserPolicyRequest
---
