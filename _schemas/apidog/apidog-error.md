---
description: Standard error response returned by the Apidog API when a request fails due to authentication issues, missing resources, or other problems.
layout: schema
name: Apidog Error
properties_list:
- description: Always false for error responses.
  name: success
  type: boolean
- description: Details about the error that occurred.
  name: error
  type: object
provider_name: Apidog
provider_slug: apidog
schema_file: json-schema/apidog-error-schema.json
slug: apidog-error
source_filename: apidog-error-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apidog/refs/heads/main/json-schema/apidog-error-schema.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Apidog Error\",\n  \"description\": \"Standard error response returned by the Apidog API when a request fails due to authentication issues, missing resources, or other problems.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"success\",\n    \"error\"\n  ],\n  \"properties\": {\n    \"success\": {\n      \"type\": \"boolean\",\n      \"description\": \"Always false for error responses.\",\n      \"const\": false\n    },\n    \"error\": {\n      \"type\": \"object\",\n      \"description\": \"Details about the error that occurred.\",\n      \"required\": [\n        \"code\",\n        \"message\"\n      ],\n      \"properties\": {\n        \"code\": {\n          \"type\": \"string\",\n          \"description\": \"A machine-readable error code.\"\n        },\n    \
  \    \"message\": {\n          \"type\": \"string\",\n          \"description\": \"A human-readable error message describing what went wrong.\"\n        }\n      },\n      \"additionalProperties\": false\n    }\n  },\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apidog/refs/heads/main/json-schema/apidog-error-schema.json
tags:
- API Design
- API Lifecycle
- API Testing
- Collaboration
- Design-First
- Documentation
- Mocking
- Platform
title: Apidog Error
---
