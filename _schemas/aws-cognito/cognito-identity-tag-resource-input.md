---
description: TagResourceInput schema from Amazon Cognito
layout: schema
name: TagResourceInput
properties_list:
- description: ''
  name: ResourceArn
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-identity-tag-resource-input-schema.json
slug: cognito-identity-tag-resource-input
source_filename: cognito-identity-tag-resource-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARNString\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the identity pool.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdentityPoolTagsType\"\n        },\n        {\n          \"description\": \"The tags to assign to the identity pool.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ResourceArn\",\n    \"Tags\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-identity-tag-resource-input-schema.json\",\n  \"title\": \"TagResourceInput\",\n  \"description\": \"TagResourceInput schema from Amazon Cognito\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-identity-tag-resource-input-schema.json
tags:
- Authentication
- Authorization
- Identity
- Identity Provider
- OAuth2
- OIDC
title: TagResourceInput
---
