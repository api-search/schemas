---
description: Returned in response to a successful GetOpenIdToken request.
layout: schema
name: GetOpenIdTokenResponse
properties_list:
- description: ''
  name: IdentityId
  type: object
- description: ''
  name: Token
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/identity-pools-get-open-id-token-response-schema.json
slug: identity-pools-get-open-id-token-response
source_filename: identity-pools-get-open-id-token-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/identity-pools-get-open-id-token-response-schema.json\",\n  \"title\": \"GetOpenIdTokenResponse\",\n  \"description\": \"Returned in response to a successful GetOpenIdToken request.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"IdentityId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdentityId\"\n        },\n        {\n          \"description\": \"A unique identifier in the format REGION:GUID. Note that the IdentityId returned may not match the one passed on input.\"\n        }\n      ]\n    },\n    \"Token\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OIDCToken\"\n        },\n        {\n          \"description\": \"An OpenID token, valid for 10 minutes.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/identity-pools-get-open-id-token-response-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: GetOpenIdTokenResponse
---
