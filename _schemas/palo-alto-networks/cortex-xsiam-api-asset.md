---
description: An asset tracked in the XSIAM asset inventory.
layout: schema
name: Asset
properties_list:
- description: ''
  name: asset_id
  type: string
- description: ''
  name: asset_name
  type: string
- description: ''
  name: asset_type
  type: string
- description: ''
  name: operating_system
  type: string
- description: ''
  name: ip_addresses
  type: array
- description: Asset risk score (0.0 to 100.0).
  name: risk_score
  type: number
- description: First observation timestamp as Unix epoch milliseconds.
  name: first_seen
  type: integer
- description: ''
  name: last_seen
  type: integer
- description: ''
  name: tags
  type: array
- description: Data sources that reported this asset.
  name: sources
  type: array
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/cortex-xsiam-api-asset-schema.json
slug: cortex-xsiam-api-asset
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Asset\",\n  \"description\": \"An asset tracked in the XSIAM asset inventory.\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cortex-xsiam-api-asset-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"asset_id\": {\n      \"type\": \"string\"\n    },\n    \"asset_name\": {\n      \"type\": \"string\"\n    },\n    \"asset_type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"DEVICE\",\n        \"CLOUD_RESOURCE\",\n        \"USER\",\n        \"SERVICE_ACCOUNT\"\n      ]\n    },\n    \"operating_system\": {\n      \"type\": \"string\"\n    },\n    \"ip_addresses\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"risk_score\": {\n      \"type\": \"number\",\n      \"description\": \"Asset risk score (0.0 to 100.0).\"\n    },\n    \"first_seen\":\
  \ {\n      \"type\": \"integer\",\n      \"description\": \"First observation timestamp as Unix epoch milliseconds.\"\n    },\n    \"last_seen\": {\n      \"type\": \"integer\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"sources\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Data sources that reported this asset.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cortex-xsiam-api-asset-schema.json
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
