---
description: ReleaseNotesList schema from Palo Alto Networks Threat Vault API
layout: schema
name: ReleaseNotesList
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
schema_file: json-schema/threat-vault-api-release-notes-list-schema.json
slug: threat-vault-api-release-notes-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ReleaseNotesList\",\n  \"description\": \"ReleaseNotesList schema from Palo Alto Networks Threat Vault API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/threat-vault-api-release-notes-list-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"success\": {\n      \"type\": \"boolean\"\n    },\n    \"data\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Content release notes for a specific PAN-OS content version.\",\n        \"properties\": {\n          \"version\": {\n            \"type\": \"string\",\n            \"description\": \"Content version identifier (e.g., 8000-7000).\"\n          },\n          \"type\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"content\",\n              \"antivirus\",\n              \"wildfire\"\
  \n            ]\n          },\n          \"release_date\": {\n            \"type\": \"string\",\n            \"format\": \"date\"\n          },\n          \"new_signatures\": {\n            \"type\": \"integer\",\n            \"description\": \"Number of new signatures in this release.\"\n          },\n          \"modified_signatures\": {\n            \"type\": \"integer\",\n            \"description\": \"Number of modified signatures in this release.\"\n          },\n          \"deprecated_signatures\": {\n            \"type\": \"integer\",\n            \"description\": \"Number of deprecated signatures in this release.\"\n          },\n          \"notes\": {\n            \"type\": \"string\",\n            \"description\": \"Release notes text.\"\n          }\n        }\n      }\n    },\n    \"total\": {\n      \"type\": \"integer\"\n    },\n    \"offset\": {\n      \"type\": \"integer\"\n    },\n    \"limit\": {\n      \"type\": \"integer\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/threat-vault-api-release-notes-list-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: ReleaseNotesList
---
