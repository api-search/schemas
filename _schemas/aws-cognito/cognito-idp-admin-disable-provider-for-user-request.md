---
description: AdminDisableProviderForUserRequest schema from Amazon Cognito
layout: schema
name: AdminDisableProviderForUserRequest
properties_list:
- description: ''
  name: UserPoolId
  type: object
- description: ''
  name: User
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-admin-disable-provider-for-user-request-schema.json
slug: cognito-idp-admin-disable-provider-for-user-request
source_filename: cognito-idp-admin-disable-provider-for-user-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"UserPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringType\"\n        },\n        {\n          \"description\": \"The user pool ID for the user pool.\"\n        }\n      ]\n    },\n    \"User\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProviderUserIdentifierType\"\n        },\n        {\n          \"description\": \"The user to be disabled.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"UserPoolId\",\n    \"User\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-admin-disable-provider-for-user-request-schema.json\",\n  \"title\": \"AdminDisableProviderForUserRequest\",\n  \"description\": \"AdminDisableProviderForUserRequest schema from Amazon Cognito\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-admin-disable-provider-for-user-request-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: AdminDisableProviderForUserRequest
---
