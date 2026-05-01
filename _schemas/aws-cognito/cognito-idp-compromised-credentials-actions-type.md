---
description: The compromised credentials actions type.
layout: schema
name: CompromisedCredentialsActionsType
properties_list:
- description: ''
  name: EventAction
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-compromised-credentials-actions-type-schema.json
slug: cognito-idp-compromised-credentials-actions-type
source_filename: cognito-idp-compromised-credentials-actions-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"EventAction\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CompromisedCredentialsEventActionType\"\n        },\n        {\n          \"description\": \"The event action.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"EventAction\"\n  ],\n  \"description\": \"The compromised credentials actions type.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-compromised-credentials-actions-type-schema.json\",\n  \"title\": \"CompromisedCredentialsActionsType\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-compromised-credentials-actions-type-schema.json
tags:
- Authentication
- Authorization
- Identity
- Identity Provider
- OAuth2
- OIDC
title: CompromisedCredentialsActionsType
---
