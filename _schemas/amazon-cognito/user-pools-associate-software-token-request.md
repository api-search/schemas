---
description: AssociateSoftwareTokenRequest schema from Amazon Cognito API
layout: schema
name: AssociateSoftwareTokenRequest
properties_list:
- description: ''
  name: AccessToken
  type: object
- description: ''
  name: Session
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-associate-software-token-request-schema.json
slug: user-pools-associate-software-token-request
source_filename: user-pools-associate-software-token-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-associate-software-token-request-schema.json\",\n  \"title\": \"AssociateSoftwareTokenRequest\",\n  \"description\": \"AssociateSoftwareTokenRequest schema from Amazon Cognito API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccessToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TokenModelType\"\n        },\n        {\n          \"description\": \"A valid access token that Amazon Cognito issued to the user whose software token you want to generate.\"\n        }\n      ]\n    },\n    \"Session\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SessionType\"\n        },\n        {\n          \"description\": \"The session that should be passed both ways in challenge-response calls to the service. This allows authentication\
  \ of the user as part of the MFA setup process.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-associate-software-token-request-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: AssociateSoftwareTokenRequest
---
