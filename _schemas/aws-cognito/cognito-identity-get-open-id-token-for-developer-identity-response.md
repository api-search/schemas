---
description: Returned in response to a successful <code>GetOpenIdTokenForDeveloperIdentity</code> request.
layout: schema
name: GetOpenIdTokenForDeveloperIdentityResponse
properties_list:
- description: ''
  name: IdentityId
  type: object
- description: ''
  name: Token
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-identity-get-open-id-token-for-developer-identity-response-schema.json
slug: cognito-identity-get-open-id-token-for-developer-identity-response
source_filename: cognito-identity-get-open-id-token-for-developer-identity-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"IdentityId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdentityId\"\n        },\n        {\n          \"description\": \"A unique identifier in the format REGION:GUID.\"\n        }\n      ]\n    },\n    \"Token\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OIDCToken\"\n        },\n        {\n          \"description\": \"An OpenID token.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Returned in response to a successful <code>GetOpenIdTokenForDeveloperIdentity</code> request.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-identity-get-open-id-token-for-developer-identity-response-schema.json\",\n  \"title\": \"GetOpenIdTokenForDeveloperIdentityResponse\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-identity-get-open-id-token-for-developer-identity-response-schema.json
tags:
- Authentication
- Authorization
- Identity
- Identity Provider
- OAuth2
- OIDC
title: GetOpenIdTokenForDeveloperIdentityResponse
---
