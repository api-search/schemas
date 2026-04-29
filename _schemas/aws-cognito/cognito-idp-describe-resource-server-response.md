---
description: DescribeResourceServerResponse schema from Amazon Cognito
layout: schema
name: DescribeResourceServerResponse
properties_list:
- description: ''
  name: ResourceServer
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-describe-resource-server-response-schema.json
slug: cognito-idp-describe-resource-server-response
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceServer\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceServerType\"\n        },\n        {\n          \"description\": \"The resource server.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ResourceServer\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-describe-resource-server-response-schema.json\",\n  \"title\": \"DescribeResourceServerResponse\",\n  \"description\": \"DescribeResourceServerResponse schema from Amazon Cognito\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-describe-resource-server-response-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: DescribeResourceServerResponse
---
