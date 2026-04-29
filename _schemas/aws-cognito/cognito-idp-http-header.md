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
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-http-header-schema.json
slug: cognito-idp-http-header
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"headerName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringType\"\n        },\n        {\n          \"description\": \"The header name.\"\n        }\n      ]\n    },\n    \"headerValue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringType\"\n        },\n        {\n          \"description\": \"The header value.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"The HTTP header.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-http-header-schema.json\",\n  \"title\": \"HttpHeader\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-http-header-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: HttpHeader
---
