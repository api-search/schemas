---
description: The challenge response type.
layout: schema
name: ChallengeResponseType
properties_list:
- description: ''
  name: ChallengeName
  type: object
- description: ''
  name: ChallengeResponse
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-challenge-response-type-schema.json
slug: cognito-idp-challenge-response-type
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ChallengeName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChallengeName\"\n        },\n        {\n          \"description\": \"The challenge name.\"\n        }\n      ]\n    },\n    \"ChallengeResponse\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChallengeResponse\"\n        },\n        {\n          \"description\": \"The challenge response.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"The challenge response type.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-challenge-response-type-schema.json\",\n  \"title\": \"ChallengeResponseType\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-challenge-response-type-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: ChallengeResponseType
---
