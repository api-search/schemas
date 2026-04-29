---
description: Input to the <code>GetIdentityPoolRoles</code> action.
layout: schema
name: GetIdentityPoolRolesInput
properties_list:
- description: ''
  name: IdentityPoolId
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-identity-get-identity-pool-roles-input-schema.json
slug: cognito-identity-get-identity-pool-roles-input
source_filename: cognito-identity-get-identity-pool-roles-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"IdentityPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdentityPoolId\"\n        },\n        {\n          \"description\": \"An identity pool ID in the format REGION:GUID.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"IdentityPoolId\"\n  ],\n  \"description\": \"Input to the <code>GetIdentityPoolRoles</code> action.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-identity-get-identity-pool-roles-input-schema.json\",\n  \"title\": \"GetIdentityPoolRolesInput\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-identity-get-identity-pool-roles-input-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: GetIdentityPoolRolesInput
---
