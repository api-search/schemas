---
description: ''
layout: schema
name: JWTValidation
properties_list:
- description: ''
  name: enabled
  type: boolean
- description: ''
  name: expires_at_validation_skew
  type: integer
- description: ''
  name: identity_base_field
  type: string
- description: ''
  name: issued_at_validation_skew
  type: integer
- description: ''
  name: not_before_validation_skew
  type: integer
- description: ''
  name: signing_method
  type: string
- description: ''
  name: source
  type: string
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-gateway-jwt-validation-schema.json
slug: tyk-gateway-jwt-validation
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"JWTValidation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"enabled\": {\n      \"type\": \"boolean\"\n    },\n    \"expires_at_validation_skew\": {\n      \"type\": \"integer\"\n    },\n    \"identity_base_field\": {\n      \"type\": \"string\"\n    },\n    \"issued_at_validation_skew\": {\n      \"type\": \"integer\"\n    },\n    \"not_before_validation_skew\": {\n      \"type\": \"integer\"\n    },\n    \"signing_method\": {\n      \"type\": \"string\"\n    },\n    \"source\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-gateway-jwt-validation-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: JWTValidation
---
