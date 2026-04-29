---
description: ChallengeResponseListType schema from Amazon Cognito
layout: schema
name: ChallengeResponseListType
properties_list: []
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-challenge-response-list-type-schema.json
slug: cognito-idp-challenge-response-list-type
source_filename: cognito-idp-challenge-response-list-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"ChallengeName\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ChallengeName\"\n          },\n          {\n            \"description\": \"The challenge name.\"\n          }\n        ]\n      },\n      \"ChallengeResponse\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ChallengeResponse\"\n          },\n          {\n            \"description\": \"The challenge response.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"The challenge response type.\"\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-challenge-response-list-type-schema.json\",\n  \"title\": \"ChallengeResponseListType\",\n  \"description\": \"ChallengeResponseListType schema from Amazon\
  \ Cognito\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-challenge-response-list-type-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: ChallengeResponseListType
---
