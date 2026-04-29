---
description: IdentifyRequestBody schema from Amplitude Identify API
layout: schema
name: IdentifyRequestBody
properties_list:
- description: The API key for the Amplitude project.
  name: api_key
  type: string
- description: An array of identification objects containing user_id or device_id and user_properties.
  name: identification
  type: array
provider_name: Amplitude
provider_slug: amplitude
schema_file: json-schema/identify-api-identify-request-body-schema.json
slug: identify-api-identify-request-body
source_filename: identify-api-identify-request-body-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/identify-api-identify-request-body-schema.json\",\n  \"title\": \"IdentifyRequestBody\",\n  \"description\": \"IdentifyRequestBody schema from Amplitude Identify API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"api_key\": {\n      \"type\": \"string\",\n      \"description\": \"The API key for the Amplitude project.\"\n    },\n    \"identification\": {\n      \"type\": \"array\",\n      \"description\": \"An array of identification objects containing user_id or device_id and user_properties.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"user_id\": {\n            \"type\": \"string\",\n            \"description\": \"A readable ID specified by you. Required unless device_id is present.\"\n          },\n          \"device_id\": {\n            \"type\":\
  \ \"string\",\n            \"description\": \"A device-specific identifier. Required unless user_id is present.\"\n          },\n          \"user_properties\": {\n            \"$ref\": \"#/components/schemas/UserPropertyOperations\"\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"api_key\",\n    \"identification\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/identify-api-identify-request-body-schema.json
tags:
- A/B Testing
- Analytics
- Experimentation
- Feature Flags
- Product Analytics
- User Behavior
title: IdentifyRequestBody
---
