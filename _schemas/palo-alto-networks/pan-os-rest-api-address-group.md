---
description: A group of address objects. Can be static with an explicit member list or dynamic with a tag-based filter expression.
layout: schema
name: AddressGroup
properties_list:
- description: Unique name of the address group.
  name: '@name'
  type: string
- description: Static address group with explicit members.
  name: static
  type: object
- description: Dynamic address group with tag-based filter.
  name: dynamic
  type: object
- description: ''
  name: description
  type: string
- description: ''
  name: tag
  type: object
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/pan-os-rest-api-address-group-schema.json
slug: pan-os-rest-api-address-group
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AddressGroup\",\n  \"description\": \"A group of address objects. Can be static with an explicit member list or dynamic with a tag-based filter expression.\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/pan-os-rest-api-address-group-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"@name\": {\n      \"type\": \"string\",\n      \"description\": \"Unique name of the address group.\"\n    },\n    \"static\": {\n      \"type\": \"object\",\n      \"description\": \"Static address group with explicit members.\",\n      \"properties\": {\n        \"member\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"List of address object names.\"\n        }\n      }\n    },\n    \"dynamic\": {\n      \"type\": \"object\",\n      \"description\"\
  : \"Dynamic address group with tag-based filter.\",\n      \"properties\": {\n        \"filter\": {\n          \"type\": \"string\",\n          \"description\": \"Tag-based filter expression (e.g., \\\"'web-servers' and 'production'\\\").\"\n        }\n      }\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"tag\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"member\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/pan-os-rest-api-address-group-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: AddressGroup
---
