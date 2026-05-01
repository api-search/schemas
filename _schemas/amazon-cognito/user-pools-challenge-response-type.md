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
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-challenge-response-type-schema.json
slug: user-pools-challenge-response-type
source_filename: user-pools-challenge-response-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-challenge-response-type-schema.json\",\n  \"title\": \"ChallengeResponseType\",\n  \"description\": \"The challenge response type.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ChallengeName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChallengeName\"\n        },\n        {\n          \"description\": \"The challenge name.\"\n        }\n      ]\n    },\n    \"ChallengeResponse\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChallengeResponse\"\n        },\n        {\n          \"description\": \"The challenge response.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-challenge-response-type-schema.json
tags:
- Authentication
- Identity
- OAuth
- User Management
title: ChallengeResponseType
---
