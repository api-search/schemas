---
description: CreateIdentityProviderResponse schema from Amazon Cognito
layout: schema
name: CreateIdentityProviderResponse
properties_list:
- description: ''
  name: IdentityProvider
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-create-identity-provider-response-schema.json
slug: cognito-idp-create-identity-provider-response
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"IdentityProvider\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdentityProviderType\"\n        },\n        {\n          \"description\": \"The newly created IdP object.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"IdentityProvider\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-create-identity-provider-response-schema.json\",\n  \"title\": \"CreateIdentityProviderResponse\",\n  \"description\": \"CreateIdentityProviderResponse schema from Amazon Cognito\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-create-identity-provider-response-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: CreateIdentityProviderResponse
---
