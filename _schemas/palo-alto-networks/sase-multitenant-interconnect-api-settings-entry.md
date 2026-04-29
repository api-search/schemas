---
description: SettingsEntry schema from SP Interconnect Manage APIs
layout: schema
name: SettingsEntry
properties_list:
- description: ''
  name: egressType
  type: string
- description: ''
  name: cidr
  type: array
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/sase-multitenant-interconnect-api-settings-entry-schema.json
slug: sase-multitenant-interconnect-api-settings-entry
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SettingsEntry\",\n  \"description\": \"SettingsEntry schema from SP Interconnect Manage APIs\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-multitenant-interconnect-api-settings-entry-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"egressType\": {\n      \"type\": \"string\",\n      \"pattern\": \"SP|PA\"\n    },\n    \"cidr\": {\n      \"type\": \"array\",\n      \"uniqueItems\": true,\n      \"items\": {\n        \"type\": \"string\",\n        \"pattern\": \"^((25[0-5]|2[0-4][0-9]|[0-1]?[0-9]{1,2})(\\\\.(25[0-5]|2[0-4][0-9]|[0-1]?[0-9]{1,2})){3})\\\\/(3[0-2]|[1-2][0-9]|[0-9])$\"\n      }\n    }\n  },\n  \"required\": [\n    \"egressType\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-multitenant-interconnect-api-settings-entry-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: SettingsEntry
---
