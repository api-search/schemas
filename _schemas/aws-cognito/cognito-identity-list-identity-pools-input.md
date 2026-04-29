---
description: Input to the ListIdentityPools action.
layout: schema
name: ListIdentityPoolsInput
properties_list:
- description: ''
  name: MaxResults
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-identity-list-identity-pools-input-schema.json
slug: cognito-identity-list-identity-pools-input
source_filename: cognito-identity-list-identity-pools-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"MaxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/QueryLimit\"\n        },\n        {\n          \"description\": \"The maximum number of identities to return.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationKey\"\n        },\n        {\n          \"description\": \"A pagination token.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"MaxResults\"\n  ],\n  \"description\": \"Input to the ListIdentityPools action.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-identity-list-identity-pools-input-schema.json\",\n  \"title\": \"ListIdentityPoolsInput\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-identity-list-identity-pools-input-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: ListIdentityPoolsInput
---
