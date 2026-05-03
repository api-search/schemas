---
description: A user within the Torii SaaS Management Platform.
layout: schema
name: Torii User
properties_list:
- description: Unique identifier for the user.
  name: id
  type: string
- description: User email address.
  name: email
  type: string
- description: First name.
  name: firstName
  type: string
- description: Last name.
  name: lastName
  type: string
- description: User status.
  name: status
  type: string
- description: Department the user belongs to.
  name: department
  type: string
- description: Whether the user is external.
  name: isExternal
  type: boolean
- description: Number of apps the user has access to.
  name: appsCount
  type: integer
- description: When the user was created.
  name: createdAt
  type: string
provider_name: Torii
provider_slug: torii
schema_file: json-schema/user.json
slug: user
source_filename: user.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/torii/refs/heads/main/json-schema/user.json\",\n  \"title\": \"Torii User\",\n  \"description\": \"A user within the Torii SaaS Management Platform.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the user.\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"User email address.\"\n    },\n    \"firstName\": {\n      \"type\": \"string\",\n      \"description\": \"First name.\"\n    },\n    \"lastName\": {\n      \"type\": \"string\",\n      \"description\": \"Last name.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"User status.\"\n    },\n    \"department\": {\n      \"type\": \"string\",\n      \"description\": \"Department the user belongs to.\"\n    },\n\
  \    \"isExternal\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user is external.\"\n    },\n    \"appsCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of apps the user has access to.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the user was created.\"\n    }\n  },\n  \"required\": [\"id\", \"email\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/torii/refs/heads/main/json-schema/user.json
tags:
- SaaS Management
title: Torii User
---
