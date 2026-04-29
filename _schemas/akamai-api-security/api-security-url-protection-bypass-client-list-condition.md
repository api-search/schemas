---
description: Collects data needed for condition matches on client lists and network lists.
layout: schema
name: url-protection-bypass-client-list-condition
properties_list:
- description: __Read-only__ Whether the connecting IP or both the connecting IP and `X-Forwarded-For` (XFF) header match on the client list or network list. URL protection bypass supports `connecting` only.
  name: checkIps
  type: string
- description: Choose `NetworkListCondition` to match the requesting client's identifier, like IP, GEO, ASN or TLS Fingerprint, against the specified client list or network list.
  name: className
  type: string
- description: __Read-only__ Whether the condition triggers on a match or lack of match.
  name: positiveMatch
  type: boolean
- description: Identifies the client list or network list.
  name: value
  type: array
provider_name: Akamai API Security
provider_slug: akamai-api-security
schema_file: json-schema/api-security-url-protection-bypass-client-list-condition-schema.json
slug: api-security-url-protection-bypass-client-list-condition
source_filename: api-security-url-protection-bypass-client-list-condition-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-url-protection-bypass-client-list-condition-schema.json\",\n  \"title\": \"url-protection-bypass-client-list-condition\",\n  \"description\": \"Collects data needed for condition matches on client lists and network lists.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"checkIps\": {\n      \"description\": \"__Read-only__ Whether the connecting IP or both the connecting IP and `X-Forwarded-For` (XFF) header match on the client list or network list. URL protection bypass supports `connecting` only.\",\n      \"enum\": [\n        \"connecting\"\n      ],\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"className\": {\n      \"description\": \"Choose `NetworkListCondition` to match the requesting client's identifier, like IP, GEO, ASN or TLS Fingerprint, against\
  \ the specified client list or network list.\",\n      \"enum\": [\n        \"NetworkListCondition\"\n      ],\n      \"type\": \"string\"\n    },\n    \"positiveMatch\": {\n      \"description\": \"__Read-only__ Whether the condition triggers on a match or lack of match.\",\n      \"readOnly\": true,\n      \"type\": \"boolean\"\n    },\n    \"value\": {\n      \"description\": \"Identifies the client list or network list.\",\n      \"items\": {\n        \"minLength\": 1,\n        \"type\": \"string\"\n      },\n      \"nullable\": true,\n      \"type\": \"array\",\n      \"uniqueItems\": true\n    }\n  },\n  \"required\": [\n    \"className\",\n    \"value\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-url-protection-bypass-client-list-condition-schema.json
tags:
- API Discovery
- API Security
- Cloud Security
- Posture Management
- Runtime Protection
- Threat Protection
title: url-protection-bypass-client-list-condition
---
