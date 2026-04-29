---
description: AssociateSoftwareTokenResponse schema from Amazon Cognito
layout: schema
name: AssociateSoftwareTokenResponse
properties_list:
- description: ''
  name: SecretCode
  type: object
- description: ''
  name: Session
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-associate-software-token-response-schema.json
slug: cognito-idp-associate-software-token-response
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"SecretCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SecretCodeType\"\n        },\n        {\n          \"description\": \"A unique generated shared secret code that is used in the TOTP algorithm to generate a one-time code.\"\n        }\n      ]\n    },\n    \"Session\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SessionType\"\n        },\n        {\n          \"description\": \"The session that should be passed both ways in challenge-response calls to the service. This allows authentication of the user as part of the MFA setup process.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-associate-software-token-response-schema.json\",\n  \"title\": \"AssociateSoftwareTokenResponse\",\n\
  \  \"description\": \"AssociateSoftwareTokenResponse schema from Amazon Cognito\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-associate-software-token-response-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: AssociateSoftwareTokenResponse
---
