---
description: The PUT Request JSON for Prefetch Requests.
layout: schema
name: prefetch-request-put
properties_list:
- description: Whether to enable prefetch requests for all extensions.
  name: allExtensions
  type: boolean
- description: Whether to enable Prefetch Requests.
  name: enableAppLayer
  type: boolean
- description: Whether to enable Prefetch Requests for rate controls.
  name: enableRateControls
  type: boolean
- description: List of extensions.
  name: extensions
  type: array
provider_name: Akamai API Security
provider_slug: akamai-api-security
schema_file: json-schema/api-security-prefetch-request-put-schema.json
slug: api-security-prefetch-request-put
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-prefetch-request-put-schema.json\",\n  \"title\": \"prefetch-request-put\",\n  \"description\": \"The PUT Request JSON for Prefetch Requests.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"allExtensions\": {\n      \"description\": \"Whether to enable prefetch requests for all extensions.\",\n      \"type\": \"boolean\"\n    },\n    \"enableAppLayer\": {\n      \"description\": \"Whether to enable Prefetch Requests.\",\n      \"type\": \"boolean\"\n    },\n    \"enableRateControls\": {\n      \"description\": \"Whether to enable Prefetch Requests for rate controls.\",\n      \"type\": \"boolean\"\n    },\n    \"extensions\": {\n      \"description\": \"List of extensions.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    }\n  },\n \
  \ \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-prefetch-request-put-schema.json
tags:
- API Discovery
- API Security
- Cloud Security
- Posture Management
- Runtime Protection
- Threat Protection
title: prefetch-request-put
---
