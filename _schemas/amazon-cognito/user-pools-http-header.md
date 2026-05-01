---
description: The HTTP header.
layout: schema
name: HttpHeader
properties_list:
- description: ''
  name: headerName
  type: object
- description: ''
  name: headerValue
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-http-header-schema.json
slug: user-pools-http-header
source_filename: user-pools-http-header-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-http-header-schema.json\",\n  \"title\": \"HttpHeader\",\n  \"description\": \"The HTTP header.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"headerName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringType\"\n        },\n        {\n          \"description\": \"The header name.\"\n        }\n      ]\n    },\n    \"headerValue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringType\"\n        },\n        {\n          \"description\": \"The header value.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-http-header-schema.json
tags:
- Authentication
- Identity
- OAuth
- User Management
title: HttpHeader
---
