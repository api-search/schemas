---
description: A Zesty.io access token provides programmatic API authentication tied to a specific role, used as an alternative to session-based authentication.
layout: schema
name: Zesty Token
properties_list:
- description: The Zesty Universal Identifier for the token.
  name: ZUID
  type: string
- description: A descriptive name for the token.
  name: name
  type: string
- description: The role ZUID this token is associated with.
  name: roleZUID
  type: string
- description: The access token value.
  name: token
  type: string
- description: Timestamp when the token was created.
  name: createdAt
  type: string
provider_name: Zesty
provider_slug: zesty
schema_file: json-schema/token.json
slug: token
source_filename: token.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/zesty/blob/main/json-schema/token.json\",\n  \"title\": \"Zesty Token\",\n  \"description\": \"A Zesty.io access token provides programmatic API authentication tied to a specific role, used as an alternative to session-based authentication.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ZUID\": {\n      \"type\": \"string\",\n      \"description\": \"The Zesty Universal Identifier for the token.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"A descriptive name for the token.\"\n    },\n    \"roleZUID\": {\n      \"type\": \"string\",\n      \"description\": \"The role ZUID this token is associated with.\"\n    },\n    \"token\": {\n      \"type\": \"string\",\n      \"description\": \"The access token value.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\"\
  : \"Timestamp when the token was created.\"\n    }\n  },\n  \"required\": [\"ZUID\", \"name\", \"roleZUID\"]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zesty/refs/heads/main/json-schema/token.json
tags:
- CMS
- Composable
- Content Management
- Headless CMS
- Media
title: Zesty Token
---
