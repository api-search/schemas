---
description: UpdateResourceServerResponse schema from Amazon Cognito
layout: schema
name: UpdateResourceServerResponse
properties_list:
- description: ''
  name: ResourceServer
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-update-resource-server-response-schema.json
slug: cognito-idp-update-resource-server-response
source_filename: cognito-idp-update-resource-server-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceServer\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceServerType\"\n        },\n        {\n          \"description\": \"The resource server.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ResourceServer\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-update-resource-server-response-schema.json\",\n  \"title\": \"UpdateResourceServerResponse\",\n  \"description\": \"UpdateResourceServerResponse schema from Amazon Cognito\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-update-resource-server-response-schema.json
tags:
- Authentication
- Authorization
- Identity
- Identity Provider
- OAuth2
- OIDC
title: UpdateResourceServerResponse
---
