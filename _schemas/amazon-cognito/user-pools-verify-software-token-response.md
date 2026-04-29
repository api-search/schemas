---
description: VerifySoftwareTokenResponse schema from Amazon Cognito API
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
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-verify-software-token-response-schema.json
slug: user-pools-verify-software-token-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-verify-software-token-response-schema.json\",\n  \"title\": \"VerifySoftwareTokenResponse\",\n  \"description\": \"VerifySoftwareTokenResponse schema from Amazon Cognito API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VerifySoftwareTokenResponseType\"\n        },\n        {\n          \"description\": \"The status of the verify software token.\"\n        }\n      ]\n    },\n    \"Session\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SessionType\"\n        },\n        {\n          \"description\": \"The session that should be passed both ways in challenge-response calls to the service.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-verify-software-token-response-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: VerifySoftwareTokenResponse
---
