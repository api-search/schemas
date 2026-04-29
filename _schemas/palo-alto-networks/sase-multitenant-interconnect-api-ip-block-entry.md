---
description: IPBlockEntry schema from SP Interconnect Manage APIs
layout: schema
name: IPBlockEntry
properties_list:
- description: ''
  name: edgeLocation
  type: string
- description: ''
  name: cidr
  type: array
- description: ''
  name: type
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/sase-multitenant-interconnect-api-ip-block-entry-schema.json
slug: sase-multitenant-interconnect-api-ip-block-entry
source_filename: sase-multitenant-interconnect-api-ip-block-entry-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"IPBlockEntry\",\n  \"description\": \"IPBlockEntry schema from SP Interconnect Manage APIs\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-multitenant-interconnect-api-ip-block-entry-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"edgeLocation\": {\n      \"type\": \"string\"\n    },\n    \"cidr\": {\n      \"type\": \"array\",\n      \"minItems\": 1,\n      \"uniqueItems\": true,\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"PRIMARY\",\n        \"SECONDARY\"\n      ]\n    }\n  },\n  \"required\": [\n    \"cidr\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-multitenant-interconnect-api-ip-block-entry-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: IPBlockEntry
---
