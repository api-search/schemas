---
description: LicenseInfo schema from Palo Alto Networks ZTNA Connector API
layout: schema
name: LicenseInfo
properties_list:
- description: Total number of ZTNA user licenses purchased.
  name: licensed_users
  type: integer
- description: Number of users actively using ZTNA.
  name: active_users
  type: integer
- description: Subscription identifier.
  name: subscription_id
  type: string
- description: Subscription expiration date and time.
  name: expires_at
  type: string
- description: List of enabled ZTNA feature entitlements.
  name: features
  type: array
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/ztna-connector-api-license-info-schema.json
slug: ztna-connector-api-license-info
source_filename: ztna-connector-api-license-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LicenseInfo\",\n  \"description\": \"LicenseInfo schema from Palo Alto Networks ZTNA Connector API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/ztna-connector-api-license-info-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"licensed_users\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of ZTNA user licenses purchased.\"\n    },\n    \"active_users\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of users actively using ZTNA.\"\n    },\n    \"subscription_id\": {\n      \"type\": \"string\",\n      \"description\": \"Subscription identifier.\"\n    },\n    \"expires_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Subscription expiration date and time.\"\n    },\n    \"features\": {\n      \"type\": \"array\",\n  \
  \    \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"List of enabled ZTNA feature entitlements.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/ztna-connector-api-license-info-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: LicenseInfo
---
