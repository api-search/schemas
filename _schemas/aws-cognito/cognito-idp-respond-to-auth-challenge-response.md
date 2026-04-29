---
description: The response to respond to the authentication challenge.
layout: schema
name: RespondToAuthChallengeResponse
properties_list:
- description: ''
  name: ChallengeName
  type: object
- description: ''
  name: Session
  type: object
- description: ''
  name: ChallengeParameters
  type: object
- description: ''
  name: AuthenticationResult
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-respond-to-auth-challenge-response-schema.json
slug: cognito-idp-respond-to-auth-challenge-response
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ChallengeName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChallengeNameType\"\n        },\n        {\n          \"description\": \"The challenge name. For more information, see <a href=\\\"https://docs.aws.amazon.com/cognito-user-identity-pools/latest/APIReference/API_InitiateAuth.html\\\">InitiateAuth</a>.\"\n        }\n      ]\n    },\n    \"Session\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SessionType\"\n        },\n        {\n          \"description\": \"The session that should be passed both ways in challenge-response calls to the service. If the caller must pass another challenge, they return a session with other challenge parameters. This session should be passed as it is to the next <code>RespondToAuthChallenge</code> API call.\"\n        }\n      ]\n    },\n    \"ChallengeParameters\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/ChallengeParametersType\"\n        },\n        {\n          \"description\": \"The challenge parameters. For more information, see <a href=\\\"https://docs.aws.amazon.com/cognito-user-identity-pools/latest/APIReference/API_InitiateAuth.html\\\">InitiateAuth</a>.\"\n        }\n      ]\n    },\n    \"AuthenticationResult\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AuthenticationResultType\"\n        },\n        {\n          \"description\": \"The result returned by the server in response to the request to respond to the authentication challenge.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"The response to respond to the authentication challenge.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-respond-to-auth-challenge-response-schema.json\",\n  \"title\": \"RespondToAuthChallengeResponse\"\
  \n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-respond-to-auth-challenge-response-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: RespondToAuthChallengeResponse
---
