---
description: An IP range owned by the organization and monitored by Xpanse.
layout: schema
name: OwnedIpRange
properties_list:
- description: ''
  name: range_id
  type: string
- description: IP range in CIDR notation (e.g., 203.0.113.0/24).
  name: cidr
  type: string
- description: ''
  name: first_ip
  type: string
- description: ''
  name: last_ip
  type: string
- description: Number of IP addresses in the range.
  name: range_size
  type: integer
- description: ''
  name: business_units
  type: array
- description: ''
  name: attribution_reason
  type: string
- description: Range creation timestamp as Unix epoch milliseconds.
  name: created
  type: integer
- description: ''
  name: modified
  type: integer
- description: ''
  name: tags
  type: array
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/cortex-xpanse-api-owned-ip-range-schema.json
slug: cortex-xpanse-api-owned-ip-range
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OwnedIpRange\",\n  \"description\": \"An IP range owned by the organization and monitored by Xpanse.\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cortex-xpanse-api-owned-ip-range-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"range_id\": {\n      \"type\": \"string\"\n    },\n    \"cidr\": {\n      \"type\": \"string\",\n      \"description\": \"IP range in CIDR notation (e.g., 203.0.113.0/24).\"\n    },\n    \"first_ip\": {\n      \"type\": \"string\"\n    },\n    \"last_ip\": {\n      \"type\": \"string\"\n    },\n    \"range_size\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of IP addresses in the range.\"\n    },\n    \"business_units\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"attribution_reason\": {\n      \"type\"\
  : \"string\",\n      \"enum\": [\n        \"RIR\",\n        \"InternallyAttributed\",\n        \"ExternallyAttributed\"\n      ]\n    },\n    \"created\": {\n      \"type\": \"integer\",\n      \"description\": \"Range creation timestamp as Unix epoch milliseconds.\"\n    },\n    \"modified\": {\n      \"type\": \"integer\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"key\": {\n            \"type\": \"string\"\n          },\n          \"value\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cortex-xpanse-api-owned-ip-range-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: OwnedIpRange
---
