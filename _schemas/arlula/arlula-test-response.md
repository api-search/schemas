---
description: Response from the API connection test endpoint.
layout: schema
name: TestResponse
properties_list:
- description: Whether the authentication was successful.
  name: success
  type: boolean
- description: Status message.
  name: message
  type: string
provider_name: Arlula
provider_slug: arlula
schema_file: json-schema/arlula-test-response-schema.json
slug: arlula-test-response
source_filename: arlula-test-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://arlula.com/json-schema/test-response.json\",\n  \"title\": \"TestResponse\",\n  \"description\": \"Response from the API connection test endpoint.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"success\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the authentication was successful.\",\n      \"examples\": [\n        true\n      ]\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Status message.\",\n      \"examples\": [\n        \"Authentication successful.\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/arlula/refs/heads/main/json-schema/arlula-test-response-schema.json
tags:
- Earth Observation
- Geospatial
- Imagery
- Remote Sensing
- Satellites
title: TestResponse
---
