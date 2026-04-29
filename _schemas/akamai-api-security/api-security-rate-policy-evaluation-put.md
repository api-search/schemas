---
description: Lists actions you can perform on a rate policy evaluation.
layout: schema
name: rate-policy-evaluation-put
properties_list:
- description: Specifies the action to perform on a rate policy evaluation, either `APPLY` or `DISCARD`.
  name: action
  type: string
provider_name: Akamai API Security
provider_slug: akamai-api-security
schema_file: json-schema/api-security-rate-policy-evaluation-put-schema.json
slug: api-security-rate-policy-evaluation-put
source_filename: api-security-rate-policy-evaluation-put-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-rate-policy-evaluation-put-schema.json\",\n  \"title\": \"rate-policy-evaluation-put\",\n  \"description\": \"Lists actions you can perform on a rate policy evaluation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"action\": {\n      \"description\": \"Specifies the action to perform on a rate policy evaluation, either `APPLY` or `DISCARD`.\",\n      \"enum\": [\n        \"APPLY\",\n        \"DISCARD\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"action\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-rate-policy-evaluation-put-schema.json
tags:
- API Discovery
- API Security
- Cloud Security
- Posture Management
- Runtime Protection
- Threat Protection
title: rate-policy-evaluation-put
---
