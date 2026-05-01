---
description: DeleteGroupRequest schema from Amazon Cognito
layout: schema
name: DeleteGroupRequest
properties_list:
- description: ''
  name: GroupName
  type: object
- description: ''
  name: UserPoolId
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-delete-group-request-schema.json
slug: cognito-idp-delete-group-request
source_filename: cognito-idp-delete-group-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"GroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GroupNameType\"\n        },\n        {\n          \"description\": \"The name of the group.\"\n        }\n      ]\n    },\n    \"UserPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolIdType\"\n        },\n        {\n          \"description\": \"The user pool ID for the user pool.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"GroupName\",\n    \"UserPoolId\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-delete-group-request-schema.json\",\n  \"title\": \"DeleteGroupRequest\",\n  \"description\": \"DeleteGroupRequest schema from Amazon Cognito\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-delete-group-request-schema.json
tags:
- Authentication
- Authorization
- Identity
- Identity Provider
- OAuth2
- OIDC
title: DeleteGroupRequest
---
