---
description: RevokeTokenRequest schema from Amazon Cognito API
layout: schema
name: RevokeTokenRequest
properties_list:
- description: ''
  name: Token
  type: object
- description: ''
  name: ClientId
  type: object
- description: ''
  name: ClientSecret
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-revoke-token-request-schema.json
slug: user-pools-revoke-token-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-revoke-token-request-schema.json\",\n  \"title\": \"RevokeTokenRequest\",\n  \"description\": \"RevokeTokenRequest schema from Amazon Cognito API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Token\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TokenModelType\"\n        },\n        {\n          \"description\": \"The refresh token that you want to revoke.\"\n        }\n      ]\n    },\n    \"ClientId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientIdType\"\n        },\n        {\n          \"description\": \"The client ID for the token that you want to revoke.\"\n        }\n      ]\n    },\n    \"ClientSecret\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientSecretType\"\n    \
  \    },\n        {\n          \"description\": \"The secret for the client ID. This is required only if the client ID has a secret.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Token\",\n    \"ClientId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-revoke-token-request-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: RevokeTokenRequest
---
