---
description: A container for the expected responses of an operation. Maps HTTP response codes to the expected response.
layout: schema
name: OpenAPI Responses Object
properties_list:
- description: ''
  name: default
  type: object
provider_name: OpenAPI
provider_slug: openapi
schema_file: json-schema/openapi-responses.json
slug: openapi-responses
source_filename: openapi-responses.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"openapi-responses.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OpenAPI Responses Object\",\n  \"description\": \"A container for the expected responses of an operation. Maps HTTP response codes to the expected response.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"default\": {\n      \"$ref\": \"openapi-response.json\"\n    }\n  },\n  \"patternProperties\": {\n    \"^[1-5](?:\\\\d{2}|XX)$\": {\n      \"$ref\": \"openapi-response.json\"\n    },\n    \"^x-\": {}\n  },\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openapi/refs/heads/main/json-schema/openapi-responses.json
tags:
- Documentation
- REST
- Specification
title: OpenAPI Responses Object
---
