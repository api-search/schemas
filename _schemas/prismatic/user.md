---
description: A user represents a person who interacts with Prismatic, either as an organization team member or a customer user.
layout: schema
name: Prismatic User
properties_list:
- description: Unique identifier for the user
  name: id
  type: string
- description: Email address of the user
  name: email
  type: string
- description: Full name of the user
  name: name
  type: string
- description: URL of the user avatar image
  name: avatarUrl
  type: string
- description: External identifier to map the user to your own system
  name: externalId
  type: string
- description: Role assigned to the user
  name: role
  type: object
- description: The customer this user belongs to, if a customer user
  name: customer
  type: object
- description: Timestamp when the user was created
  name: createdAt
  type: string
- description: Timestamp when the user was last updated
  name: updatedAt
  type: string
provider_name: Prismatic
provider_slug: prismatic
schema_file: json-schema/user.json
slug: user
source_filename: user.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/prismatic/refs/heads/main/json-schema/user.json\",\n  \"title\": \"Prismatic User\",\n  \"description\": \"A user represents a person who interacts with Prismatic, either as an organization team member or a customer user.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"email\", \"name\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the user\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Email address of the user\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Full name of the user\"\n    },\n    \"avatarUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the user avatar image\"\n    },\n    \"externalId\": {\n      \"type\":\
  \ \"string\",\n      \"description\": \"External identifier to map the user to your own system\"\n    },\n    \"role\": {\n      \"type\": \"object\",\n      \"description\": \"Role assigned to the user\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"enum\": [\"Owner\", \"Admin\", \"Member\", \"Guest\", \"Third Party\"]\n        }\n      }\n    },\n    \"customer\": {\n      \"$ref\": \"customer.json\",\n      \"description\": \"The customer this user belongs to, if a customer user\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the user was created\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the user was last updated\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/prismatic/refs/heads/main/json-schema/user.json
tags:
- Embedded iPaaS
- Integrations
- Workflows
title: Prismatic User
---
