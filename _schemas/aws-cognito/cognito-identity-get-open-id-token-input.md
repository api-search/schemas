---
description: Input to the GetOpenIdToken action.
layout: schema
name: GetOpenIdTokenInput
properties_list:
- description: ''
  name: IdentityId
  type: object
- description: ''
  name: Logins
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-identity-get-open-id-token-input-schema.json
slug: cognito-identity-get-open-id-token-input
source_filename: cognito-identity-get-open-id-token-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"IdentityId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdentityId\"\n        },\n        {\n          \"description\": \"A unique identifier in the format REGION:GUID.\"\n        }\n      ]\n    },\n    \"Logins\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LoginsMap\"\n        },\n        {\n          \"description\": \"A set of optional name-value pairs that map provider names to provider tokens. When using graph.facebook.com and www.amazon.com, supply the access_token returned from the provider's authflow. For accounts.google.com, an Amazon Cognito user pool provider, or any other OpenID Connect provider, always include the <code>id_token</code>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"IdentityId\"\n  ],\n  \"description\": \"Input to the GetOpenIdToken action.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\"\
  ,\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-identity-get-open-id-token-input-schema.json\",\n  \"title\": \"GetOpenIdTokenInput\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-identity-get-open-id-token-input-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: GetOpenIdTokenInput
---
