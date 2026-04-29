---
description: The compromised credentials actions type.
layout: schema
name: CompromisedCredentialsActionsType
properties_list:
- description: ''
  name: EventAction
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-compromised-credentials-actions-type-schema.json
slug: user-pools-compromised-credentials-actions-type
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-compromised-credentials-actions-type-schema.json\",\n  \"title\": \"CompromisedCredentialsActionsType\",\n  \"description\": \"The compromised credentials actions type.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EventAction\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CompromisedCredentialsEventActionType\"\n        },\n        {\n          \"description\": \"The event action.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"EventAction\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-compromised-credentials-actions-type-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: CompromisedCredentialsActionsType
---
