---
description: Returned in response to a successful <code>GetCredentialsForIdentity</code> operation.
layout: schema
name: GetCredentialsForIdentityResponse
properties_list:
- description: ''
  name: IdentityId
  type: object
- description: ''
  name: Credentials
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-identity-get-credentials-for-identity-response-schema.json
slug: cognito-identity-get-credentials-for-identity-response
source_filename: cognito-identity-get-credentials-for-identity-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"IdentityId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdentityId\"\n        },\n        {\n          \"description\": \"A unique identifier in the format REGION:GUID.\"\n        }\n      ]\n    },\n    \"Credentials\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Credentials\"\n        },\n        {\n          \"description\": \"Credentials for the provided identity ID.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Returned in response to a successful <code>GetCredentialsForIdentity</code> operation.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-identity-get-credentials-for-identity-response-schema.json\",\n  \"title\": \"GetCredentialsForIdentityResponse\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-identity-get-credentials-for-identity-response-schema.json
tags:
- Authentication
- Authorization
- Identity
- Identity Provider
- OAuth2
- OIDC
title: GetCredentialsForIdentityResponse
---
