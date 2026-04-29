---
description: BuilderInfo schema from Ampersand API
layout: schema
name: BuilderInfo
properties_list:
- description: ''
  name: builder
  type: object
- description: A map of project IDs to project roles for the builder.
  name: projectRoles
  type: object
- description: ''
  name: orgRole
  type: object
provider_name: Ampersand
provider_slug: ampersand
schema_file: json-schema/ampersand-api-builder-info-schema.json
slug: ampersand-api-builder-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-builder-info-schema.json\",\n  \"title\": \"BuilderInfo\",\n  \"description\": \"BuilderInfo schema from Ampersand API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"builder\": {\n      \"$ref\": \"#/components/schemas/Builder\"\n    },\n    \"projectRoles\": {\n      \"type\": \"object\",\n      \"description\": \"A map of project IDs to project roles for the builder.\",\n      \"additionalProperties\": {\n        \"type\": \"object\",\n        \"required\": [\n          \"role\",\n          \"principalType\",\n          \"principalId\",\n          \"project\"\n        ],\n        \"properties\": {\n          \"role\": {\n            \"type\": \"string\",\n            \"description\": \"The role of the builder in the project.\",\n            \"example\": \"admin\"\n          },\n    \
  \      \"principalType\": {\n            \"type\": \"string\",\n            \"description\": \"The type of the principal.\",\n            \"enum\": [\n              \"team\",\n              \"builder\"\n            ]\n          },\n          \"principalId\": {\n            \"type\": \"string\",\n            \"description\": \"The ID of the team or builder.\",\n            \"example\": \"builder-id-123\"\n          },\n          \"project\": {\n            \"$ref\": \"#/components/schemas/Project\"\n          }\n        }\n      }\n    },\n    \"orgRole\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"role\",\n        \"principalType\",\n        \"principalId\",\n        \"org\"\n      ],\n      \"properties\": {\n        \"role\": {\n          \"type\": \"string\",\n          \"description\": \"The role of the builder in the org.\",\n          \"example\": \"admin\"\n        },\n        \"principalType\": {\n          \"type\": \"string\",\n          \"description\"\
  : \"The type of the principal.\",\n          \"enum\": [\n            \"team\",\n            \"builder\"\n          ]\n        },\n        \"principalId\": {\n          \"type\": \"string\",\n          \"description\": \"The ID of the team or builder.\",\n          \"example\": \"builder-id-123\"\n        },\n        \"org\": {\n          \"$ref\": \"#/components/schemas/Org\"\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"builder\",\n    \"projectRoles\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-builder-info-schema.json
tags:
- Developer Tools
- Integrations
- Platform
- SaaS
- OAuth
- Data Sync
- Webhooks
title: BuilderInfo
---
