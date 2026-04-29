---
description: Contains bypass network lists for the specified configuration version.
layout: schema
name: bypass-network-lists-get
properties_list:
- description: The list of network list identifiers and names.
  name: networkLists
  type: array
provider_name: Akamai API Security
provider_slug: akamai-api-security
schema_file: json-schema/api-security-bypass-network-lists-get-schema.json
slug: api-security-bypass-network-lists-get
source_filename: api-security-bypass-network-lists-get-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-bypass-network-lists-get-schema.json\",\n  \"title\": \"bypass-network-lists-get\",\n  \"description\": \"Contains bypass network lists for the specified configuration version.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"networkLists\": {\n      \"description\": \"The list of network list identifiers and names.\",\n      \"items\": {\n        \"additionalProperties\": false,\n        \"properties\": {\n          \"id\": {\n            \"description\": \"Uniquely identifies the network list.\",\n            \"type\": \"string\"\n          },\n          \"name\": {\n            \"description\": \"The name of the network list.\",\n            \"type\": \"string\"\n          }\n        },\n        \"required\": [\n          \"id\"\n        ],\n        \"type\": \"object\"\n   \
  \   },\n      \"type\": \"array\"\n    }\n  },\n  \"required\": [\n    \"networkLists\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-bypass-network-lists-get-schema.json
tags:
- API Discovery
- API Security
- Cloud Security
- Posture Management
- Runtime Protection
- Threat Protection
title: bypass-network-lists-get
---
