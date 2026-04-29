---
description: Account takeover actions type.
layout: schema
name: AccountTakeoverActionsType
properties_list:
- description: ''
  name: LowAction
  type: object
- description: ''
  name: MediumAction
  type: object
- description: ''
  name: HighAction
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-account-takeover-actions-type-schema.json
slug: user-pools-account-takeover-actions-type
source_filename: user-pools-account-takeover-actions-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-account-takeover-actions-type-schema.json\",\n  \"title\": \"AccountTakeoverActionsType\",\n  \"description\": \"Account takeover actions type.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"LowAction\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountTakeoverActionType\"\n        },\n        {\n          \"description\": \"Action to take for a low risk.\"\n        }\n      ]\n    },\n    \"MediumAction\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountTakeoverActionType\"\n        },\n        {\n          \"description\": \"Action to take for a medium risk.\"\n        }\n      ]\n    },\n    \"HighAction\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountTakeoverActionType\"\n\
  \        },\n        {\n          \"description\": \"Action to take for a high risk.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-account-takeover-actions-type-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: AccountTakeoverActionsType
---
