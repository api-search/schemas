---
description: Represents the request to change a user password.
layout: schema
name: ChangePasswordRequest
properties_list:
- description: ''
  name: PreviousPassword
  type: object
- description: ''
  name: ProposedPassword
  type: object
- description: ''
  name: AccessToken
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-change-password-request-schema.json
slug: cognito-idp-change-password-request
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"PreviousPassword\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PasswordType\"\n        },\n        {\n          \"description\": \"The old password.\"\n        }\n      ]\n    },\n    \"ProposedPassword\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PasswordType\"\n        },\n        {\n          \"description\": \"The new password.\"\n        }\n      ]\n    },\n    \"AccessToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TokenModelType\"\n        },\n        {\n          \"description\": \"A valid access token that Amazon Cognito issued to the user whose password you want to change.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"PreviousPassword\",\n    \"ProposedPassword\",\n    \"AccessToken\"\n  ],\n  \"description\": \"Represents the request to change a user password.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\"\
  ,\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-change-password-request-schema.json\",\n  \"title\": \"ChangePasswordRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-change-password-request-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: ChangePasswordRequest
---
