---
description: ListTagsForResourceInput schema from Amazon Cognito
layout: schema
name: ListTagsForResourceInput
properties_list:
- description: ''
  name: ResourceArn
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-identity-list-tags-for-resource-input-schema.json
slug: cognito-identity-list-tags-for-resource-input
source_filename: cognito-identity-list-tags-for-resource-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARNString\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the identity pool that the tags are assigned to.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ResourceArn\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-identity-list-tags-for-resource-input-schema.json\",\n  \"title\": \"ListTagsForResourceInput\",\n  \"description\": \"ListTagsForResourceInput schema from Amazon Cognito\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-identity-list-tags-for-resource-input-schema.json
tags:
- Authentication
- Authorization
- Identity
- Identity Provider
- OAuth2
- OIDC
title: ListTagsForResourceInput
---
