---
description: ListIdentityProvidersResponse schema from Amazon Cognito
layout: schema
name: ListIdentityProvidersResponse
properties_list:
- description: ''
  name: Providers
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-list-identity-providers-response-schema.json
slug: cognito-idp-list-identity-providers-response
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Providers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProvidersListType\"\n        },\n        {\n          \"description\": \"A list of IdP objects.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationKeyType\"\n        },\n        {\n          \"description\": \"A pagination token.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Providers\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-list-identity-providers-response-schema.json\",\n  \"title\": \"ListIdentityProvidersResponse\",\n  \"description\": \"ListIdentityProvidersResponse schema from Amazon Cognito\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-list-identity-providers-response-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: ListIdentityProvidersResponse
---
