---
description: UntagResourceRequest schema from Amazon Cognito
layout: schema
name: UntagResourceRequest
properties_list:
- description: ''
  name: ResourceArn
  type: object
- description: ''
  name: TagKeys
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-untag-resource-request-schema.json
slug: cognito-idp-untag-resource-request
source_filename: cognito-idp-untag-resource-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArnType\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the user pool that the tags are assigned to.\"\n        }\n      ]\n    },\n    \"TagKeys\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolTagsListType\"\n        },\n        {\n          \"description\": \"The keys of the tags to remove from the user pool.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ResourceArn\",\n    \"TagKeys\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-untag-resource-request-schema.json\",\n  \"title\": \"UntagResourceRequest\",\n  \"description\": \"UntagResourceRequest schema from Amazon Cognito\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-untag-resource-request-schema.json
tags:
- Authentication
- Authorization
- Identity
- Identity Provider
- OAuth2
- OIDC
title: UntagResourceRequest
---
