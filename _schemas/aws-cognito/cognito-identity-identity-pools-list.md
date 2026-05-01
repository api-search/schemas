---
description: IdentityPoolsList schema from Amazon Cognito
layout: schema
name: IdentityPoolsList
properties_list: []
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-identity-identity-pools-list-schema.json
slug: cognito-identity-identity-pools-list
source_filename: cognito-identity-identity-pools-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"IdentityPoolId\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/IdentityPoolId\"\n          },\n          {\n            \"description\": \"An identity pool ID in the format REGION:GUID.\"\n          }\n        ]\n      },\n      \"IdentityPoolName\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/IdentityPoolName\"\n          },\n          {\n            \"description\": \"A string that you provide.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"A description of the identity pool.\"\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-identity-identity-pools-list-schema.json\",\n  \"title\": \"IdentityPoolsList\",\n  \"description\": \"IdentityPoolsList schema\
  \ from Amazon Cognito\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-identity-identity-pools-list-schema.json
tags:
- Authentication
- Authorization
- Identity
- Identity Provider
- OAuth2
- OIDC
title: IdentityPoolsList
---
