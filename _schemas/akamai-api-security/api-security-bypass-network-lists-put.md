---
description: Contains bypass network lists for the specified configuration version.
layout: schema
name: bypass-network-lists-put
properties_list:
- description: Contains a list of network list IDs.
  name: networkLists
  type: array
provider_name: Akamai API Security
provider_slug: akamai-api-security
schema_file: json-schema/api-security-bypass-network-lists-put-schema.json
slug: api-security-bypass-network-lists-put
source_filename: api-security-bypass-network-lists-put-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-bypass-network-lists-put-schema.json\",\n  \"title\": \"bypass-network-lists-put\",\n  \"description\": \"Contains bypass network lists for the specified configuration version.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"networkLists\": {\n      \"description\": \"Contains a list of network list IDs.\",\n      \"items\": {\n        \"description\": \"List of network lists. The values are the network lists' IDs.\",\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    }\n  },\n  \"required\": [\n    \"networkLists\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-bypass-network-lists-put-schema.json
tags:
- API Discovery
- API Security
- Cloud Security
- Posture Management
- Runtime Protection
- Threat Protection
title: bypass-network-lists-put
---
