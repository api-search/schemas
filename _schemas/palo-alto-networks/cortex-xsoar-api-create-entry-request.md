---
description: CreateEntryRequest schema from Palo Alto Networks Cortex XSOAR REST API
layout: schema
name: CreateEntryRequest
properties_list:
- description: ID of the investigation to add the entry to.
  name: investigationId
  type: string
- description: Entry content text or command to execute.
  name: data
  type: string
- description: Whether to render the content as Markdown.
  name: markdown
  type: boolean
- description: ''
  name: tags
  type: array
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/cortex-xsoar-api-create-entry-request-schema.json
slug: cortex-xsoar-api-create-entry-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateEntryRequest\",\n  \"description\": \"CreateEntryRequest schema from Palo Alto Networks Cortex XSOAR REST API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cortex-xsoar-api-create-entry-request-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"investigationId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the investigation to add the entry to.\"\n    },\n    \"data\": {\n      \"type\": \"string\",\n      \"description\": \"Entry content text or command to execute.\"\n    },\n    \"markdown\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to render the content as Markdown.\",\n      \"default\": false\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n    \"investigationId\"\
  ,\n    \"data\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cortex-xsoar-api-create-entry-request-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: CreateEntryRequest
---
