---
description: A description of the identity pool.
layout: schema
name: IdentityPoolShortDescription
properties_list:
- description: ''
  name: IdentityPoolId
  type: object
- description: ''
  name: IdentityPoolName
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-identity-identity-pool-short-description-schema.json
slug: cognito-identity-identity-pool-short-description
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"IdentityPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdentityPoolId\"\n        },\n        {\n          \"description\": \"An identity pool ID in the format REGION:GUID.\"\n        }\n      ]\n    },\n    \"IdentityPoolName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdentityPoolName\"\n        },\n        {\n          \"description\": \"A string that you provide.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"A description of the identity pool.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-identity-identity-pool-short-description-schema.json\",\n  \"title\": \"IdentityPoolShortDescription\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-identity-identity-pool-short-description-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: IdentityPoolShortDescription
---
