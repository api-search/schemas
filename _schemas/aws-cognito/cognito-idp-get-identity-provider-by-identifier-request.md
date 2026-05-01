---
description: GetIdentityProviderByIdentifierRequest schema from Amazon Cognito
layout: schema
name: GetIdentityProviderByIdentifierRequest
properties_list:
- description: ''
  name: UserPoolId
  type: object
- description: ''
  name: IdpIdentifier
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-get-identity-provider-by-identifier-request-schema.json
slug: cognito-idp-get-identity-provider-by-identifier-request
source_filename: cognito-idp-get-identity-provider-by-identifier-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"UserPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolIdType\"\n        },\n        {\n          \"description\": \"The user pool ID.\"\n        }\n      ]\n    },\n    \"IdpIdentifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdpIdentifierType\"\n        },\n        {\n          \"description\": \"The IdP identifier.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"UserPoolId\",\n    \"IdpIdentifier\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-get-identity-provider-by-identifier-request-schema.json\",\n  \"title\": \"GetIdentityProviderByIdentifierRequest\",\n  \"description\": \"GetIdentityProviderByIdentifierRequest schema from Amazon Cognito\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-get-identity-provider-by-identifier-request-schema.json
tags:
- Authentication
- Authorization
- Identity
- Identity Provider
- OAuth2
- OIDC
title: GetIdentityProviderByIdentifierRequest
---
