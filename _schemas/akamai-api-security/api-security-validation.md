---
description: Contains feedback on validation.
layout: schema
name: validation
properties_list:
- description: The explanation of the error message.
  name: detail
  type: string
- description: The name of the field causing the validation problem.
  name: fieldName
  type: string
- description: The JSON reference to the field in the resource.
  name: jsonReference
  type: string
- description: The title for the error.
  name: title
  type: string
- description: The URL for the error type.
  name: type
  type: string
provider_name: Akamai API Security
provider_slug: akamai-api-security
schema_file: json-schema/api-security-validation-schema.json
slug: api-security-validation
source_filename: api-security-validation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-validation-schema.json\",\n  \"title\": \"validation\",\n  \"description\": \"Contains feedback on validation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"detail\": {\n      \"description\": \"The explanation of the error message.\",\n      \"type\": \"string\"\n    },\n    \"fieldName\": {\n      \"description\": \"The name of the field causing the validation problem.\",\n      \"type\": \"string\"\n    },\n    \"jsonReference\": {\n      \"description\": \"The JSON reference to the field in the resource.\",\n      \"type\": \"string\"\n    },\n    \"title\": {\n      \"description\": \"The title for the error.\",\n      \"example\": \"Not Found\",\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"description\": \"The URL for the error type.\",\n      \"example\"\
  : \"/appsec/problem-types/INCOMPATIBLE-FIELD\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"title\",\n    \"type\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-validation-schema.json
tags:
- API Discovery
- API Security
- Cloud Security
- Posture Management
- Runtime Protection
- Threat Protection
title: validation
---
