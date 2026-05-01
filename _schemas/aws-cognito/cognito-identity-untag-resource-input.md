---
description: UntagResourceInput schema from Amazon Cognito
layout: schema
name: UntagResourceInput
properties_list:
- description: ''
  name: ResourceArn
  type: object
- description: ''
  name: TagKeys
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-identity-untag-resource-input-schema.json
slug: cognito-identity-untag-resource-input
source_filename: cognito-identity-untag-resource-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARNString\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the identity pool.\"\n        }\n      ]\n    },\n    \"TagKeys\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdentityPoolTagsListType\"\n        },\n        {\n          \"description\": \"The keys of the tags to remove from the user pool.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ResourceArn\",\n    \"TagKeys\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-identity-untag-resource-input-schema.json\",\n  \"title\": \"UntagResourceInput\",\n  \"description\": \"UntagResourceInput schema from Amazon Cognito\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-identity-untag-resource-input-schema.json
tags:
- Authentication
- Authorization
- Identity
- Identity Provider
- OAuth2
- OIDC
title: UntagResourceInput
---
