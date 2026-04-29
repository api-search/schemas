---
description: Represents the response to describe the user pool.
layout: schema
name: DescribeUserPoolResponse
properties_list:
- description: ''
  name: UserPool
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-describe-user-pool-response-schema.json
slug: cognito-idp-describe-user-pool-response
source_filename: cognito-idp-describe-user-pool-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"UserPool\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolType\"\n        },\n        {\n          \"description\": \"The container of metadata returned by the server to describe the pool.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Represents the response to describe the user pool.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-describe-user-pool-response-schema.json\",\n  \"title\": \"DescribeUserPoolResponse\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-describe-user-pool-response-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: DescribeUserPoolResponse
---
