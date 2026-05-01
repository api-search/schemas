---
description: DeleteResourceServerRequest schema from Amazon Cognito
layout: schema
name: DeleteResourceServerRequest
properties_list:
- description: ''
  name: UserPoolId
  type: object
- description: ''
  name: Identifier
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-delete-resource-server-request-schema.json
slug: cognito-idp-delete-resource-server-request
source_filename: cognito-idp-delete-resource-server-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"UserPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolIdType\"\n        },\n        {\n          \"description\": \"The user pool ID for the user pool that hosts the resource server.\"\n        }\n      ]\n    },\n    \"Identifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceServerIdentifierType\"\n        },\n        {\n          \"description\": \"The identifier for the resource server.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"UserPoolId\",\n    \"Identifier\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-delete-resource-server-request-schema.json\",\n  \"title\": \"DeleteResourceServerRequest\",\n  \"description\": \"DeleteResourceServerRequest schema from Amazon Cognito\"\
  \n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-delete-resource-server-request-schema.json
tags:
- Authentication
- Authorization
- Identity
- Identity Provider
- OAuth2
- OIDC
title: DeleteResourceServerRequest
---
