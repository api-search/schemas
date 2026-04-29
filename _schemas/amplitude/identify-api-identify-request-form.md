---
description: IdentifyRequestForm schema from Amplitude Identify API
layout: schema
name: IdentifyRequestForm
properties_list:
- description: The API key for the Amplitude project.
  name: api_key
  type: string
- description: A JSON-encoded string or array of JSON-encoded identification objects containing user_id or device_id and user_properties.
  name: identification
  type: string
provider_name: Amplitude
provider_slug: amplitude
schema_file: json-schema/identify-api-identify-request-form-schema.json
slug: identify-api-identify-request-form
source_filename: identify-api-identify-request-form-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/identify-api-identify-request-form-schema.json\",\n  \"title\": \"IdentifyRequestForm\",\n  \"description\": \"IdentifyRequestForm schema from Amplitude Identify API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"api_key\": {\n      \"type\": \"string\",\n      \"description\": \"The API key for the Amplitude project.\"\n    },\n    \"identification\": {\n      \"type\": \"string\",\n      \"description\": \"A JSON-encoded string or array of JSON-encoded identification objects containing user_id or device_id and user_properties.\"\n    }\n  },\n  \"required\": [\n    \"api_key\",\n    \"identification\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/identify-api-identify-request-form-schema.json
tags:
- A/B Testing
- Analytics
- Experimentation
- Feature Flags
- Product Analytics
- User Behavior
title: IdentifyRequestForm
---
