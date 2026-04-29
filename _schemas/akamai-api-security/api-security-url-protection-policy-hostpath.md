---
description: The hostname and path combinations to match on.
layout: schema
name: url-protection-policy-hostpath
properties_list:
- description: The hostnames you choose to match on.
  name: hostname
  type: string
- description: The list of paths to match on.
  name: paths
  type: array
provider_name: Akamai API Security
provider_slug: akamai-api-security
schema_file: json-schema/api-security-url-protection-policy-hostpath-schema.json
slug: api-security-url-protection-policy-hostpath
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-url-protection-policy-hostpath-schema.json\",\n  \"title\": \"url-protection-policy-hostpath\",\n  \"description\": \"The hostname and path combinations to match on.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"hostname\": {\n      \"description\": \"The hostnames you choose to match on.\",\n      \"type\": \"string\"\n    },\n    \"paths\": {\n      \"description\": \"The list of paths to match on.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    }\n  },\n  \"required\": [\n    \"hostname\",\n    \"paths\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-url-protection-policy-hostpath-schema.json
tags:
- API Discovery
- API Security
- Cloud Security
- Posture Management
- Runtime Protection
- Threat Protection
title: url-protection-policy-hostpath
---
