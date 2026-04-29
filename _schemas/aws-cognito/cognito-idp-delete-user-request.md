---
description: Represents the request to delete a user.
layout: schema
name: DeleteUserRequest
properties_list:
- description: ''
  name: AccessToken
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-delete-user-request-schema.json
slug: cognito-idp-delete-user-request
source_filename: cognito-idp-delete-user-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccessToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TokenModelType\"\n        },\n        {\n          \"description\": \"A valid access token that Amazon Cognito issued to the user whose user profile you want to delete.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AccessToken\"\n  ],\n  \"description\": \"Represents the request to delete a user.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-delete-user-request-schema.json\",\n  \"title\": \"DeleteUserRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-delete-user-request-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: DeleteUserRequest
---
