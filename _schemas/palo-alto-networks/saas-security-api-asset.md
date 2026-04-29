---
description: Asset schema from Palo Alto Networks SaaS Security API
layout: schema
name: Asset
properties_list:
- description: Unique asset identifier.
  name: id
  type: string
- description: Asset name or filename.
  name: name
  type: string
- description: Asset type.
  name: type
  type: string
- description: ID of the SaaS application containing the asset.
  name: app_id
  type: string
- description: Name of the SaaS application.
  name: app_name
  type: string
- description: User ID of the asset owner.
  name: owner
  type: string
- description: Current exposure level of the asset.
  name: exposure
  type: string
- description: Asset size in bytes.
  name: size_bytes
  type: integer
- description: DLP policy violation names triggered for this asset.
  name: dlp_violations
  type: array
- description: ''
  name: created_at
  type: string
- description: ''
  name: updated_at
  type: string
- description: ''
  name: last_scanned_at
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/saas-security-api-asset-schema.json
slug: saas-security-api-asset
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Asset\",\n  \"description\": \"Asset schema from Palo Alto Networks SaaS Security API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/saas-security-api-asset-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique asset identifier.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Asset name or filename.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"file\",\n        \"folder\",\n        \"email\",\n        \"calendar_event\",\n        \"contact\"\n      ],\n      \"description\": \"Asset type.\"\n    },\n    \"app_id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the SaaS application containing the asset.\"\n    },\n    \"app_name\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"Name of the SaaS application.\"\n    },\n    \"owner\": {\n      \"type\": \"string\",\n      \"description\": \"User ID of the asset owner.\"\n    },\n    \"exposure\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"private\",\n        \"internal\",\n        \"external\",\n        \"public\"\n      ],\n      \"description\": \"Current exposure level of the asset.\"\n    },\n    \"size_bytes\": {\n      \"type\": \"integer\",\n      \"description\": \"Asset size in bytes.\"\n    },\n    \"dlp_violations\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"DLP policy violation names triggered for this asset.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"last_scanned_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\
  \n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/saas-security-api-asset-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: Asset
---
