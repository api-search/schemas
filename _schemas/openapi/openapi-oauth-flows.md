---
description: Allows configuration of the supported OAuth Flows.
layout: schema
name: OpenAPI OAuth Flows Object
properties_list:
- description: ''
  name: implicit
  type: object
- description: ''
  name: password
  type: object
- description: ''
  name: clientCredentials
  type: object
- description: ''
  name: authorizationCode
  type: object
provider_name: OpenAPI
provider_slug: openapi
schema_file: json-schema/openapi-oauth-flows.json
slug: openapi-oauth-flows
source_filename: openapi-oauth-flows.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"openapi-oauth-flows.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OpenAPI OAuth Flows Object\",\n  \"description\": \"Allows configuration of the supported OAuth Flows.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"implicit\": {\n      \"$ref\": \"openapi-oauth-flow.json\"\n    },\n    \"password\": {\n      \"$ref\": \"openapi-oauth-flow.json\"\n    },\n    \"clientCredentials\": {\n      \"$ref\": \"openapi-oauth-flow.json\"\n    },\n    \"authorizationCode\": {\n      \"$ref\": \"openapi-oauth-flow.json\"\n    }\n  },\n  \"patternProperties\": {\n    \"^x-\": {}\n  },\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openapi/refs/heads/main/json-schema/openapi-oauth-flows.json
tags:
- Documentation
- REST
- Specification
title: OpenAPI OAuth Flows Object
---
