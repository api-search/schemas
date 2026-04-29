---
description: GetPrincipalTagAttributeMapInput schema from Amazon Cognito
layout: schema
name: GetPrincipalTagAttributeMapInput
properties_list:
- description: ''
  name: IdentityPoolId
  type: object
- description: ''
  name: IdentityProviderName
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-identity-get-principal-tag-attribute-map-input-schema.json
slug: cognito-identity-get-principal-tag-attribute-map-input
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"IdentityPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdentityPoolId\"\n        },\n        {\n          \"description\": \"You can use this operation to get the ID of the Identity Pool you setup attribute mappings for.\"\n        }\n      ]\n    },\n    \"IdentityProviderName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdentityProviderName\"\n        },\n        {\n          \"description\": \"You can use this operation to get the provider name.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"IdentityPoolId\",\n    \"IdentityProviderName\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-identity-get-principal-tag-attribute-map-input-schema.json\",\n  \"title\": \"GetPrincipalTagAttributeMapInput\"\
  ,\n  \"description\": \"GetPrincipalTagAttributeMapInput schema from Amazon Cognito\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-identity-get-principal-tag-attribute-map-input-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: GetPrincipalTagAttributeMapInput
---
