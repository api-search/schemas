---
description: Input to the <code>UnlinkDeveloperIdentity</code> action.
layout: schema
name: UnlinkDeveloperIdentityInput
properties_list:
- description: ''
  name: IdentityId
  type: object
- description: ''
  name: IdentityPoolId
  type: object
- description: ''
  name: DeveloperProviderName
  type: object
- description: ''
  name: DeveloperUserIdentifier
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-identity-unlink-developer-identity-input-schema.json
slug: cognito-identity-unlink-developer-identity-input
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"IdentityId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdentityId\"\n        },\n        {\n          \"description\": \"A unique identifier in the format REGION:GUID.\"\n        }\n      ]\n    },\n    \"IdentityPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdentityPoolId\"\n        },\n        {\n          \"description\": \"An identity pool ID in the format REGION:GUID.\"\n        }\n      ]\n    },\n    \"DeveloperProviderName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeveloperProviderName\"\n        },\n        {\n          \"description\": \"The \\\"domain\\\" by which Cognito will refer to your users.\"\n        }\n      ]\n    },\n    \"DeveloperUserIdentifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeveloperUserIdentifier\"\n        },\n        {\n          \"\
  description\": \"A unique ID used by your backend authentication process to identify a user.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"IdentityId\",\n    \"IdentityPoolId\",\n    \"DeveloperProviderName\",\n    \"DeveloperUserIdentifier\"\n  ],\n  \"description\": \"Input to the <code>UnlinkDeveloperIdentity</code> action.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-identity-unlink-developer-identity-input-schema.json\",\n  \"title\": \"UnlinkDeveloperIdentityInput\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-identity-unlink-developer-identity-input-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: UnlinkDeveloperIdentityInput
---
