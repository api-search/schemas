---
description: Represents the request to describe a user pool client.
layout: schema
name: DescribeUserPoolClientRequest
properties_list:
- description: ''
  name: UserPoolId
  type: object
- description: ''
  name: ClientId
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-describe-user-pool-client-request-schema.json
slug: cognito-idp-describe-user-pool-client-request
source_filename: cognito-idp-describe-user-pool-client-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"UserPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolIdType\"\n        },\n        {\n          \"description\": \"The user pool ID for the user pool you want to describe.\"\n        }\n      ]\n    },\n    \"ClientId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientIdType\"\n        },\n        {\n          \"description\": \"The app client ID of the app associated with the user pool.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"UserPoolId\",\n    \"ClientId\"\n  ],\n  \"description\": \"Represents the request to describe a user pool client.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-describe-user-pool-client-request-schema.json\",\n  \"title\": \"DescribeUserPoolClientRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-describe-user-pool-client-request-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: DescribeUserPoolClientRequest
---
