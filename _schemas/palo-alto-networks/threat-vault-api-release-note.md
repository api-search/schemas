---
description: Content release notes for a specific PAN-OS content version.
layout: schema
name: ReleaseNote
properties_list:
- description: Content version identifier (e.g., 8000-7000).
  name: version
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: release_date
  type: string
- description: Number of new signatures in this release.
  name: new_signatures
  type: integer
- description: Number of modified signatures in this release.
  name: modified_signatures
  type: integer
- description: Number of deprecated signatures in this release.
  name: deprecated_signatures
  type: integer
- description: Release notes text.
  name: notes
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/threat-vault-api-release-note-schema.json
slug: threat-vault-api-release-note
source_filename: threat-vault-api-release-note-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ReleaseNote\",\n  \"description\": \"Content release notes for a specific PAN-OS content version.\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/threat-vault-api-release-note-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"Content version identifier (e.g., 8000-7000).\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"content\",\n        \"antivirus\",\n        \"wildfire\"\n      ]\n    },\n    \"release_date\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"new_signatures\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of new signatures in this release.\"\n    },\n    \"modified_signatures\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of\
  \ modified signatures in this release.\"\n    },\n    \"deprecated_signatures\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of deprecated signatures in this release.\"\n    },\n    \"notes\": {\n      \"type\": \"string\",\n      \"description\": \"Release notes text.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/threat-vault-api-release-note-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: ReleaseNote
---
