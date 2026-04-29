---
description: Builder schema from Ampersand API
layout: schema
name: Builder
properties_list:
- description: The builder ID.
  name: id
  type: string
- description: The identity provider
  name: idpProvider
  type: string
- description: ID used by the identity provider
  name: idpRef
  type: string
- description: The time that the builder joined Ampersand.
  name: createTime
  type: string
- description: ''
  name: firstName
  type: string
- description: ''
  name: lastName
  type: string
- description: ''
  name: fullName
  type: string
- description: ''
  name: primaryEmail
  type: string
provider_name: Ampersand
provider_slug: ampersand
schema_file: json-schema/ampersand-api-builder-schema.json
slug: ampersand-api-builder
source_filename: ampersand-api-builder-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-builder-schema.json\",\n  \"title\": \"Builder\",\n  \"description\": \"Builder schema from Ampersand API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The builder ID.\",\n      \"example\": \"builder-id-123\"\n    },\n    \"idpProvider\": {\n      \"type\": \"string\",\n      \"description\": \"The identity provider\",\n      \"example\": \"clerk\"\n    },\n    \"idpRef\": {\n      \"type\": \"string\",\n      \"description\": \"ID used by the identity provider\"\n    },\n    \"createTime\": {\n      \"type\": \"string\",\n      \"description\": \"The time that the builder joined Ampersand.\",\n      \"format\": \"date-time\"\n    },\n    \"firstName\": {\n      \"type\": \"string\"\n    },\n    \"lastName\": {\n      \"\
  type\": \"string\"\n    },\n    \"fullName\": {\n      \"type\": \"string\"\n    },\n    \"primaryEmail\": {\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"idpProvider\",\n    \"idpRef\",\n    \"createTime\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-builder-schema.json
tags:
- Developer Tools
- Integrations
- Platform
- SaaS
- OAuth
- Data Sync
- Webhooks
title: Builder
---
