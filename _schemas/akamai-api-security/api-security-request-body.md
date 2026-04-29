---
description: Contains the size limits for a request body.
layout: schema
name: request-body
properties_list:
- description: Request body size in KB, either `8`, `16`, or `32` as string-formatted integers, or `default` to use Akamai's best practice value.
  name: requestBodyInspectionLimitInKB
  type: string
provider_name: Akamai API Security
provider_slug: akamai-api-security
schema_file: json-schema/api-security-request-body-schema.json
slug: api-security-request-body
source_filename: api-security-request-body-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-request-body-schema.json\",\n  \"title\": \"request-body\",\n  \"description\": \"Contains the size limits for a request body.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"requestBodyInspectionLimitInKB\": {\n      \"description\": \"Request body size in KB, either `8`, `16`, or `32` as string-formatted integers, or `default` to use Akamai's best practice value.\",\n      \"enum\": [\n        \"8\",\n        \"16\",\n        \"32\",\n        \"default\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-request-body-schema.json
tags:
- API Discovery
- API Security
- Cloud Security
- Posture Management
- Runtime Protection
- Threat Protection
title: request-body
---
