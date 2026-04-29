---
description: A Cortex XSOAR integration pack providing connectivity to a third-party tool.
layout: schema
name: Integration
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: name
  type: string
- description: Human-readable display name.
  name: display
  type: string
- description: Integration category (e.g., Endpoint, Firewall, SIEM).
  name: category
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: version
  type: integer
- description: ''
  name: fromVersion
  type: string
- description: ''
  name: deprecated
  type: boolean
- description: ''
  name: beta
  type: boolean
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/cortex-xsoar-api-integration-schema.json
slug: cortex-xsoar-api-integration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Integration\",\n  \"description\": \"A Cortex XSOAR integration pack providing connectivity to a third-party tool.\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cortex-xsoar-api-integration-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"display\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable display name.\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Integration category (e.g., Endpoint, Firewall, SIEM).\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"version\": {\n      \"type\": \"integer\"\n    },\n    \"fromVersion\": {\n      \"type\": \"string\"\n    },\n    \"deprecated\": {\n      \"type\": \"boolean\"\
  \n    },\n    \"beta\": {\n      \"type\": \"boolean\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cortex-xsoar-api-integration-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: Integration
---
