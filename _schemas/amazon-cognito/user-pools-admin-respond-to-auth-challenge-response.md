---
description: Responds to the authentication challenge, as an administrator.
layout: schema
name: AdminRespondToAuthChallengeResponse
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
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-admin-respond-to-auth-challenge-response-schema.json
slug: user-pools-admin-respond-to-auth-challenge-response
source_filename: user-pools-admin-respond-to-auth-challenge-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-admin-respond-to-auth-challenge-response-schema.json\",\n  \"title\": \"AdminRespondToAuthChallengeResponse\",\n  \"description\": \"Responds to the authentication challenge, as an administrator.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ChallengeName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChallengeNameType\"\n        },\n        {\n          \"description\": \"The name of the challenge. For more information, see <a href=\\\"https://docs.aws.amazon.com/cognito-user-identity-pools/latest/APIReference/API_AdminInitiateAuth.html\\\">AdminInitiateAuth</a>.\"\n        }\n      ]\n    },\n    \"Session\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SessionType\"\n        },\n        {\n          \"description\"\
  : \"The session that should be passed both ways in challenge-response calls to the service. If the caller must pass another challenge, they return a session with other challenge parameters. This session should be passed as it is to the next <code>RespondToAuthChallenge</code> API call.\"\n        }\n      ]\n    },\n    \"ChallengeParameters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChallengeParametersType\"\n        },\n        {\n          \"description\": \"The challenge parameters. For more information, see <a href=\\\"https://docs.aws.amazon.com/cognito-user-identity-pools/latest/APIReference/API_AdminInitiateAuth.html\\\">AdminInitiateAuth</a>.\"\n        }\n      ]\n    },\n    \"AuthenticationResult\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AuthenticationResultType\"\n        },\n        {\n          \"description\": \"The result returned by the server in response to the authentication request.\"\n    \
  \    }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-admin-respond-to-auth-challenge-response-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: AdminRespondToAuthChallengeResponse
---
