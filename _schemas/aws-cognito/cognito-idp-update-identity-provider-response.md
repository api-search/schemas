---
description: UpdateIdentityProviderResponse schema from Amazon Cognito
layout: schema
name: UpdateIdentityProviderResponse
properties_list:
- description: ''
  name: IdentityProvider
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-update-identity-provider-response-schema.json
slug: cognito-idp-update-identity-provider-response
source_filename: cognito-idp-update-identity-provider-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"IdentityProvider\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdentityProviderType\"\n        },\n        {\n          \"description\": \"The identity provider details.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"IdentityProvider\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-update-identity-provider-response-schema.json\",\n  \"title\": \"UpdateIdentityProviderResponse\",\n  \"description\": \"UpdateIdentityProviderResponse schema from Amazon Cognito\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-update-identity-provider-response-schema.json
tags:
- Authentication
- Authorization
- Identity
- Identity Provider
- OAuth2
- OIDC
title: UpdateIdentityProviderResponse
---
