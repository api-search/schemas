---
description: A historical record of a signature version.
layout: schema
name: ThreatHistoryEntry
properties_list:
- description: ''
  name: id
  type: integer
- description: ''
  name: name
  type: string
- description: Content version number for this history entry.
  name: version
  type: string
- description: ''
  name: release_time
  type: string
- description: ''
  name: action
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/threat-vault-api-threat-history-entry-schema.json
slug: threat-vault-api-threat-history-entry
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ThreatHistoryEntry\",\n  \"description\": \"A historical record of a signature version.\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/threat-vault-api-threat-history-entry-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"Content version number for this history entry.\"\n    },\n    \"release_time\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"action\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"added\",\n        \"modified\",\n        \"deprecated\"\n      ]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/threat-vault-api-threat-history-entry-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: ThreatHistoryEntry
---
