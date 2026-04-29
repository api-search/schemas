---
description: IPPoolRequest schema from SP Interconnect Manage APIs
layout: schema
name: IPPoolRequest
properties_list:
- description: ''
  name: ipBlocks
  type: array
- description: ''
  name: ipProvider
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/sase-multitenant-interconnect-api-ip-pool-request-schema.json
slug: sase-multitenant-interconnect-api-ip-pool-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"IPPoolRequest\",\n  \"description\": \"IPPoolRequest schema from SP Interconnect Manage APIs\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-multitenant-interconnect-api-ip-pool-request-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ipBlocks\": {\n      \"type\": \"array\",\n      \"uniqueItems\": true,\n      \"items\": {\n        \"type\": \"object\",\n        \"required\": [\n          \"cidr\"\n        ],\n        \"properties\": {\n          \"edgeLocation\": {\n            \"type\": \"string\"\n          },\n          \"cidr\": {\n            \"type\": \"array\",\n            \"minItems\": 1,\n            \"uniqueItems\": true,\n            \"items\": {\n              \"type\": \"string\"\n            }\n          },\n          \"type\": {\n            \"type\": \"string\",\n            \"enum\"\
  : [\n              \"PRIMARY\",\n              \"SECONDARY\"\n            ]\n          }\n        }\n      }\n    },\n    \"ipProvider\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"SP\",\n        \"PANW\"\n      ]\n    }\n  },\n  \"required\": [\n    \"ipProvider\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-multitenant-interconnect-api-ip-pool-request-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: IPPoolRequest
---
