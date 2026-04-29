---
description: Represents the response from the server to the request to create the user.
layout: schema
name: AdminCreateUserResponse
properties_list:
- description: ''
  name: User
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-admin-create-user-response-schema.json
slug: cognito-idp-admin-create-user-response
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"User\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserType\"\n        },\n        {\n          \"description\": \"The newly created user.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Represents the response from the server to the request to create the user.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-admin-create-user-response-schema.json\",\n  \"title\": \"AdminCreateUserResponse\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-admin-create-user-response-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: AdminCreateUserResponse
---
