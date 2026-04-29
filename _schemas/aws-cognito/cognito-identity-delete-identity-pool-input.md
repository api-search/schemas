---
description: Input to the DeleteIdentityPool action.
layout: schema
name: DeleteIdentityPoolInput
properties_list:
- description: ''
  name: IdentityPoolId
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-identity-delete-identity-pool-input-schema.json
slug: cognito-identity-delete-identity-pool-input
source_filename: cognito-identity-delete-identity-pool-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"IdentityPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdentityPoolId\"\n        },\n        {\n          \"description\": \"An identity pool ID in the format REGION:GUID.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"IdentityPoolId\"\n  ],\n  \"description\": \"Input to the DeleteIdentityPool action.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-identity-delete-identity-pool-input-schema.json\",\n  \"title\": \"DeleteIdentityPoolInput\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-identity-delete-identity-pool-input-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: DeleteIdentityPoolInput
---
