---
description: A group of address objects. Can be static with an explicit member list or dynamic with a tag-based filter expression.
layout: schema
name: AddressGroup
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: folder
  type: string
- description: List of address object names for static groups.
  name: static
  type: array
- description: ''
  name: dynamic
  type: object
- description: ''
  name: description
  type: string
- description: ''
  name: tag
  type: array
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/strata-cloud-manager-api-address-group-schema.json
slug: strata-cloud-manager-api-address-group
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AddressGroup\",\n  \"description\": \"A group of address objects. Can be static with an explicit member list or dynamic with a tag-based filter expression.\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/strata-cloud-manager-api-address-group-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"readOnly\": true\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"folder\": {\n      \"type\": \"string\",\n      \"readOnly\": true\n    },\n    \"static\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"List of address object names for static groups.\"\n    },\n    \"dynamic\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"filter\": {\n   \
  \       \"type\": \"string\",\n          \"description\": \"Tag-based filter expression (e.g., \\\"'web-servers' and 'production'\\\").\"\n        }\n      }\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"tag\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/strata-cloud-manager-api-address-group-schema.json
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
