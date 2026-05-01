---
description: Input to the <code>DeleteIdentities</code> action.
layout: schema
name: DeleteIdentitiesInput
properties_list:
- description: ''
  name: IdentityIdsToDelete
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-identity-delete-identities-input-schema.json
slug: cognito-identity-delete-identities-input
source_filename: cognito-identity-delete-identities-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"IdentityIdsToDelete\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdentityIdList\"\n        },\n        {\n          \"description\": \"A list of 1-60 identities that you want to delete.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"IdentityIdsToDelete\"\n  ],\n  \"description\": \"Input to the <code>DeleteIdentities</code> action.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-identity-delete-identities-input-schema.json\",\n  \"title\": \"DeleteIdentitiesInput\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-identity-delete-identities-input-schema.json
tags:
- Authentication
- Authorization
- Identity
- Identity Provider
- OAuth2
- OIDC
title: DeleteIdentitiesInput
---
