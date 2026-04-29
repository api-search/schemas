---
description: ContentSnippet schema from Palo Alto Networks Enterprise DLP API
layout: schema
name: ContentSnippet
properties_list:
- description: Data pattern identifier that matched.
  name: pattern_id
  type: string
- description: Data pattern name that matched.
  name: pattern_name
  type: string
- description: Context snippet around the data pattern match.
  name: snippet
  type: string
- description: Character offset position of the match within the document.
  name: position
  type: integer
- description: Whether the matched content within the snippet is masked.
  name: masked
  type: boolean
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/dlp-api-content-snippet-schema.json
slug: dlp-api-content-snippet
source_filename: dlp-api-content-snippet-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ContentSnippet\",\n  \"description\": \"ContentSnippet schema from Palo Alto Networks Enterprise DLP API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/dlp-api-content-snippet-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"pattern_id\": {\n      \"type\": \"string\",\n      \"description\": \"Data pattern identifier that matched.\"\n    },\n    \"pattern_name\": {\n      \"type\": \"string\",\n      \"description\": \"Data pattern name that matched.\"\n    },\n    \"snippet\": {\n      \"type\": \"string\",\n      \"description\": \"Context snippet around the data pattern match.\"\n    },\n    \"position\": {\n      \"type\": \"integer\",\n      \"description\": \"Character offset position of the match within the document.\"\n    },\n    \"masked\": {\n      \"type\": \"boolean\",\n      \"description\": \"\
  Whether the matched content within the snippet is masked.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/dlp-api-content-snippet-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: ContentSnippet
---
