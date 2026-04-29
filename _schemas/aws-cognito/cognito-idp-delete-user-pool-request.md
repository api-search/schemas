---
description: Represents the request to delete a user pool.
layout: schema
name: DeleteUserPoolRequest
properties_list:
- description: ''
  name: UserPoolId
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-delete-user-pool-request-schema.json
slug: cognito-idp-delete-user-pool-request
source_filename: cognito-idp-delete-user-pool-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"UserPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolIdType\"\n        },\n        {\n          \"description\": \"The user pool ID for the user pool you want to delete.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"UserPoolId\"\n  ],\n  \"description\": \"Represents the request to delete a user pool.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-delete-user-pool-request-schema.json\",\n  \"title\": \"DeleteUserPoolRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-delete-user-pool-request-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: DeleteUserPoolRequest
---
