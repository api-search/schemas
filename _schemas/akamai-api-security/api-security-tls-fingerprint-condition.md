---
description: Collects data needed for condition matches on TLS fingerprints.
layout: schema
name: tls-fingerprint-condition
properties_list:
- description: The type of condition. In this case, `TlsFingerprintCondition`.
  name: className
  type: string
- description: Whether the condition triggers on a match or lack of match.
  name: positiveMatch
  type: boolean
- description: A list of unique TLS fingerprints.
  name: value
  type: array
provider_name: Akamai API Security
provider_slug: akamai-api-security
schema_file: json-schema/api-security-tls-fingerprint-condition-schema.json
slug: api-security-tls-fingerprint-condition
source_filename: api-security-tls-fingerprint-condition-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-tls-fingerprint-condition-schema.json\",\n  \"title\": \"tls-fingerprint-condition\",\n  \"description\": \"Collects data needed for condition matches on TLS fingerprints.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"className\": {\n      \"description\": \"The type of condition. In this case, `TlsFingerprintCondition`.\",\n      \"enum\": [\n        \"TlsFingerprintCondition\"\n      ],\n      \"type\": \"string\"\n    },\n    \"positiveMatch\": {\n      \"description\": \"Whether the condition triggers on a match or lack of match.\",\n      \"type\": \"boolean\"\n    },\n    \"value\": {\n      \"description\": \"A list of unique TLS fingerprints.\",\n      \"items\": {\n        \"minLength\": 1,\n        \"type\": \"string\"\n      },\n      \"minItems\": 1,\n      \"type\"\
  : \"array\",\n      \"uniqueItems\": true\n    }\n  },\n  \"required\": [\n    \"className\",\n    \"value\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-tls-fingerprint-condition-schema.json
tags:
- API Discovery
- API Security
- Cloud Security
- Posture Management
- Runtime Protection
- Threat Protection
title: tls-fingerprint-condition
---
