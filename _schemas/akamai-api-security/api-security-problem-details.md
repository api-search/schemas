---
description: Details the errors you can receive.
layout: schema
name: problem-details
properties_list:
- description: The detailed error message.
  name: detail
  type: string
- description: Pointers to fields for which invalid input was provided, whose values are messages detailing the reason this input was invalid for this field.
  name: fieldErrors
  type: object
- description: The non-referenceable URI that indicates the error instance.
  name: instance
  type: string
- description: The HTTP status code.
  name: status
  type: integer
- description: The error title.
  name: title
  type: string
- description: The URL for the error type.
  name: type
  type: string
provider_name: Akamai API Security
provider_slug: akamai-api-security
schema_file: json-schema/api-security-problem-details-schema.json
slug: api-security-problem-details
source_filename: api-security-problem-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-problem-details-schema.json\",\n  \"title\": \"problem-details\",\n  \"description\": \"Details the errors you can receive.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"detail\": {\n      \"description\": \"The detailed error message.\",\n      \"type\": \"string\"\n    },\n    \"fieldErrors\": {\n      \"additionalProperties\": {\n        \"description\": \"Fields that provide additional details about the problem.\",\n        \"type\": \"string\"\n      },\n      \"description\": \"Pointers to fields for which invalid input was provided, whose values are messages detailing the reason this input was invalid for this field.\",\n      \"type\": \"object\"\n    },\n    \"instance\": {\n      \"description\": \"The non-referenceable URI that indicates the error instance.\",\n  \
  \    \"example\": \"https://problems.luna.akamaiapis.net/api-definitions/error-instances/d54686b5-21cb-4ab7-a8d6-a92282cf1749\",\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"description\": \"The HTTP status code.\",\n      \"example\": 404,\n      \"type\": \"integer\"\n    },\n    \"title\": {\n      \"description\": \"The error title.\",\n      \"example\": \"Not Found\",\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"description\": \"The URL for the error type.\",\n      \"example\": \"https://problems.luna.akamaiapis.net/api-definitions/error-types/NOT-FOUND\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"title\",\n    \"type\",\n    \"detail\",\n    \"instance\",\n    \"status\"\n  ],\n  \"additionalProperties\": true\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-problem-details-schema.json
tags:
- API Discovery
- API Security
- Cloud Security
- Posture Management
- Runtime Protection
- Threat Protection
title: problem-details
---
