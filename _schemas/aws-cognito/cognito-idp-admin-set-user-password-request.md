---
description: AdminSetUserPasswordRequest schema from Amazon Cognito
layout: schema
name: AdminSetUserPasswordRequest
properties_list:
- description: ''
  name: UserPoolId
  type: object
- description: ''
  name: Username
  type: object
- description: ''
  name: Password
  type: object
- description: ''
  name: Permanent
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-admin-set-user-password-request-schema.json
slug: cognito-idp-admin-set-user-password-request
source_filename: cognito-idp-admin-set-user-password-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"UserPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolIdType\"\n        },\n        {\n          \"description\": \"The user pool ID for the user pool where you want to set the user's password.\"\n        }\n      ]\n    },\n    \"Username\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UsernameType\"\n        },\n        {\n          \"description\": \"The user name of the user whose password you want to set.\"\n        }\n      ]\n    },\n    \"Password\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PasswordType\"\n        },\n        {\n          \"description\": \"The password for the user.\"\n        }\n      ]\n    },\n    \"Permanent\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BooleanType\"\n        },\n        {\n          \"description\": \" <code>True</code> if the password\
  \ is permanent, <code>False</code> if it is temporary.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"UserPoolId\",\n    \"Username\",\n    \"Password\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-admin-set-user-password-request-schema.json\",\n  \"title\": \"AdminSetUserPasswordRequest\",\n  \"description\": \"AdminSetUserPasswordRequest schema from Amazon Cognito\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-admin-set-user-password-request-schema.json
tags:
- Authentication
- Authorization
- Identity
- Identity Provider
- OAuth2
- OIDC
title: AdminSetUserPasswordRequest
---
