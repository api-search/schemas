---
description: Schema for the CompleteDNS v2 DNS history response.
layout: schema
name: CompleteDNS DNS History
properties_list:
- description: The queried domain name.
  name: domain
  type: string
- description: Total nameserver drop events.
  name: drops
  type: integer
- description: Total nameserver change events.
  name: changes
  type: integer
- description: Years of history tracked.
  name: years
  type: number
- description: Whether the domain was ever parked.
  name: was_parked
  type: boolean
- description: ''
  name: events
  type: array
provider_name: CompleteDNS
provider_slug: completedns
schema_file: json-schema/completedns-dns-history-schema.json
slug: completedns-dns-history
source_filename: completedns-dns-history-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/completedns/main/json-schema/completedns-dns-history-schema.json\",\n  \"title\": \"CompleteDNS DNS History\",\n  \"description\": \"Schema for the CompleteDNS v2 DNS history response.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"domain\": {\n      \"type\": \"string\",\n      \"description\": \"The queried domain name.\"\n    },\n    \"drops\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"Total nameserver drop events.\"\n    },\n    \"changes\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"Total nameserver change events.\"\n    },\n    \"years\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"description\": \"Years of history tracked.\"\n    },\n    \"was_parked\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the domain was ever\
  \ parked.\"\n    },\n    \"events\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/event\"\n      }\n    }\n  },\n  \"required\": [\"domain\", \"events\"],\n  \"$defs\": {\n    \"event\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"date\": { \"type\": \"string\" },\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\"start_tracking\", \"dropped\", \"created\", \"change\"]\n        },\n        \"nameservers\": {\n          \"type\": \"array\",\n          \"items\": { \"type\": \"string\" }\n        },\n        \"changes\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"action\": { \"type\": \"string\", \"enum\": [\"added\", \"removed\"] },\n              \"nameserver\": { \"type\": \"string\" }\n            }\n          }\n        }\n      },\n      \"required\": [\"type\"]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/completedns/refs/heads/main/json-schema/completedns-dns-history-schema.json
tags:
- DNS
- DNS History
- Domain Intelligence
- Domains
- Nameservers
- Threat Intelligence
title: CompleteDNS DNS History
---
