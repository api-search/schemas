---
description: VerifySoftwareTokenResponse schema from Amazon Cognito
layout: schema
name: VerifySoftwareTokenResponse
properties_list:
- description: ''
  name: Status
  type: object
- description: ''
  name: Session
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-verify-software-token-response-schema.json
slug: cognito-idp-verify-software-token-response
source_filename: cognito-idp-verify-software-token-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VerifySoftwareTokenResponseType\"\n        },\n        {\n          \"description\": \"The status of the verify software token.\"\n        }\n      ]\n    },\n    \"Session\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SessionType\"\n        },\n        {\n          \"description\": \"The session that should be passed both ways in challenge-response calls to the service.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-verify-software-token-response-schema.json\",\n  \"title\": \"VerifySoftwareTokenResponse\",\n  \"description\": \"VerifySoftwareTokenResponse schema from Amazon Cognito\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-verify-software-token-response-schema.json
tags:
- Authentication
- Authorization
- Identity
- Identity Provider
- OAuth2
- OIDC
title: VerifySoftwareTokenResponse
---
