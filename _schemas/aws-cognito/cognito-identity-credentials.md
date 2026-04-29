---
description: Credentials for the provided identity ID.
layout: schema
name: Credentials
properties_list:
- description: ''
  name: AccessKeyId
  type: object
- description: ''
  name: SecretKey
  type: object
- description: ''
  name: SessionToken
  type: object
- description: ''
  name: Expiration
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-identity-credentials-schema.json
slug: cognito-identity-credentials
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccessKeyId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccessKeyString\"\n        },\n        {\n          \"description\": \"The Access Key portion of the credentials.\"\n        }\n      ]\n    },\n    \"SecretKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SecretKeyString\"\n        },\n        {\n          \"description\": \"The Secret Access Key portion of the credentials\"\n        }\n      ]\n    },\n    \"SessionToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SessionTokenString\"\n        },\n        {\n          \"description\": \"The Session Token portion of the credentials\"\n        }\n      ]\n    },\n    \"Expiration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateType\"\n        },\n        {\n          \"description\": \"The date at which these credentials will\
  \ expire.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Credentials for the provided identity ID.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-identity-credentials-schema.json\",\n  \"title\": \"Credentials\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-identity-credentials-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: Credentials
---
