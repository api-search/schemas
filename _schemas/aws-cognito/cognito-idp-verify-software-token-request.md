---
description: VerifySoftwareTokenRequest schema from Amazon Cognito
layout: schema
name: VerifySoftwareTokenRequest
properties_list:
- description: ''
  name: AccessToken
  type: object
- description: ''
  name: Session
  type: object
- description: ''
  name: UserCode
  type: object
- description: ''
  name: FriendlyDeviceName
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-verify-software-token-request-schema.json
slug: cognito-idp-verify-software-token-request
source_filename: cognito-idp-verify-software-token-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccessToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TokenModelType\"\n        },\n        {\n          \"description\": \"A valid access token that Amazon Cognito issued to the user whose software token you want to verify.\"\n        }\n      ]\n    },\n    \"Session\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SessionType\"\n        },\n        {\n          \"description\": \"The session that should be passed both ways in challenge-response calls to the service.\"\n        }\n      ]\n    },\n    \"UserCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SoftwareTokenMFAUserCodeType\"\n        },\n        {\n          \"description\": \"The one- time password computed using the secret code returned by <a href=\\\"https://docs.aws.amazon.com/cognito-user-identity-pools/latest/APIReference/API_AssociateSoftwareToken.html\\\
  \">AssociateSoftwareToken</a>.\"\n        }\n      ]\n    },\n    \"FriendlyDeviceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringType\"\n        },\n        {\n          \"description\": \"The friendly device name.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"UserCode\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-verify-software-token-request-schema.json\",\n  \"title\": \"VerifySoftwareTokenRequest\",\n  \"description\": \"VerifySoftwareTokenRequest schema from Amazon Cognito\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-verify-software-token-request-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: VerifySoftwareTokenRequest
---
