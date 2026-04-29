---
description: CloudAccount schema from Palo Alto Networks Prisma Cloud CSPM API
layout: schema
name: CloudAccount
properties_list:
- description: Cloud provider account identifier.
  name: accountId
  type: string
- description: Display name of the account.
  name: name
  type: string
- description: Cloud provider type.
  name: cloudType
  type: string
- description: Whether monitoring is enabled.
  name: enabled
  type: boolean
- description: Number of policies applied to this account.
  name: numberOfPolicies
  type: integer
- description: Epoch timestamp of last modification.
  name: lastModifiedTs
  type: integer
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-cloud-cspm-api-cloud-account-schema.json
slug: prisma-cloud-cspm-api-cloud-account
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CloudAccount\",\n  \"description\": \"CloudAccount schema from Palo Alto Networks Prisma Cloud CSPM API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-cspm-api-cloud-account-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountId\": {\n      \"type\": \"string\",\n      \"description\": \"Cloud provider account identifier.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the account.\"\n    },\n    \"cloudType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"aws\",\n        \"azure\",\n        \"gcp\",\n        \"oci\"\n      ],\n      \"description\": \"Cloud provider type.\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether monitoring is enabled.\"\n    },\n    \"numberOfPolicies\": {\n\
  \      \"type\": \"integer\",\n      \"description\": \"Number of policies applied to this account.\"\n    },\n    \"lastModifiedTs\": {\n      \"type\": \"integer\",\n      \"description\": \"Epoch timestamp of last modification.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-cspm-api-cloud-account-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: CloudAccount
---
