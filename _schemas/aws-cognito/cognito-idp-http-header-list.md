---
description: HttpHeaderList schema from Amazon Cognito
layout: schema
name: HttpHeaderList
properties_list: []
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-http-header-list-schema.json
slug: cognito-idp-http-header-list
source_filename: cognito-idp-http-header-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"headerName\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/StringType\"\n          },\n          {\n            \"description\": \"The header name.\"\n          }\n        ]\n      },\n      \"headerValue\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/StringType\"\n          },\n          {\n            \"description\": \"The header value.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"The HTTP header.\"\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-http-header-list-schema.json\",\n  \"title\": \"HttpHeaderList\",\n  \"description\": \"HttpHeaderList schema from Amazon Cognito\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-http-header-list-schema.json
tags:
- Authentication
- Authorization
- Identity
- Identity Provider
- OAuth2
- OIDC
title: HttpHeaderList
---
