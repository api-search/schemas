---
description: You can use this parameter to set an MFA configuration that uses the SMS delivery medium.
layout: schema
name: AdminSetUserSettingsRequest
properties_list:
- description: ''
  name: UserPoolId
  type: object
- description: ''
  name: Username
  type: object
- description: ''
  name: MFAOptions
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-admin-set-user-settings-request-schema.json
slug: cognito-idp-admin-set-user-settings-request
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"UserPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolIdType\"\n        },\n        {\n          \"description\": \"The ID of the user pool that contains the user whose options you're setting.\"\n        }\n      ]\n    },\n    \"Username\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UsernameType\"\n        },\n        {\n          \"description\": \"The user name of the user whose options you're setting.\"\n        }\n      ]\n    },\n    \"MFAOptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MFAOptionListType\"\n        },\n        {\n          \"description\": \"You can use this parameter only to set an SMS configuration that uses SMS for delivery.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"UserPoolId\",\n    \"Username\",\n    \"MFAOptions\"\n  ],\n  \"description\": \"You can use this\
  \ parameter to set an MFA configuration that uses the SMS delivery medium.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-admin-set-user-settings-request-schema.json\",\n  \"title\": \"AdminSetUserSettingsRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-admin-set-user-settings-request-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: AdminSetUserSettingsRequest
---
