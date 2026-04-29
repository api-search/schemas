---
description: ThreatHistoryList schema from Palo Alto Networks Threat Vault API
layout: schema
name: ThreatHistoryList
properties_list:
- description: ''
  name: success
  type: boolean
- description: ''
  name: data
  type: array
- description: ''
  name: total
  type: integer
- description: ''
  name: offset
  type: integer
- description: ''
  name: limit
  type: integer
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/threat-vault-api-threat-history-list-schema.json
slug: threat-vault-api-threat-history-list
source_filename: threat-vault-api-threat-history-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ThreatHistoryList\",\n  \"description\": \"ThreatHistoryList schema from Palo Alto Networks Threat Vault API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/threat-vault-api-threat-history-list-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"success\": {\n      \"type\": \"boolean\"\n    },\n    \"data\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"A historical record of a signature version.\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"integer\"\n          },\n          \"name\": {\n            \"type\": \"string\"\n          },\n          \"version\": {\n            \"type\": \"string\",\n            \"description\": \"Content version number for this history entry.\"\n          },\n          \"release_time\": {\n\
  \            \"type\": \"string\",\n            \"format\": \"date-time\"\n          },\n          \"action\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"added\",\n              \"modified\",\n              \"deprecated\"\n            ]\n          }\n        }\n      }\n    },\n    \"total\": {\n      \"type\": \"integer\"\n    },\n    \"offset\": {\n      \"type\": \"integer\"\n    },\n    \"limit\": {\n      \"type\": \"integer\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/threat-vault-api-threat-history-list-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: ThreatHistoryList
---
