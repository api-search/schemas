---
description: A user account in a Retool organization with role-based access control.
layout: schema
name: Retool User
properties_list:
- description: The unique UUID identifier for the user.
  name: id
  type: string
- description: The user's email address, unique within the organization.
  name: email
  type: string
- description: The user's first name.
  name: firstName
  type: string
- description: The user's last name.
  name: lastName
  type: string
- description: Whether the user has administrator privileges.
  name: isAdmin
  type: boolean
- description: Whether the user account is disabled.
  name: isDisabled
  type: boolean
- description: The user type determining default access level.
  name: userType
  type: string
- description: Groups the user belongs to.
  name: groups
  type: array
- description: Timestamp when the user was created.
  name: createdAt
  type: string
- description: Timestamp when the user was last updated.
  name: updatedAt
  type: string
provider_name: Retool
provider_slug: retool
schema_file: json-schema/retool-user-schema.json
slug: retool-user
source_filename: retool-user-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/retool/json-schema/retool-user-schema.json\",\n  \"title\": \"Retool User\",\n  \"description\": \"A user account in a Retool organization with role-based access control.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"email\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The unique UUID identifier for the user.\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"The user's email address, unique within the organization.\"\n    },\n    \"firstName\": {\n      \"type\": \"string\",\n      \"description\": \"The user's first name.\"\n    },\n    \"lastName\": {\n      \"type\": \"string\",\n      \"description\": \"The user's last name.\"\n    },\n    \"isAdmin\": {\n      \"type\": \"boolean\",\n      \"description\": \"\
  Whether the user has administrator privileges.\",\n      \"default\": false\n    },\n    \"isDisabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user account is disabled.\",\n      \"default\": false\n    },\n    \"userType\": {\n      \"type\": \"string\",\n      \"description\": \"The user type determining default access level.\",\n      \"enum\": [\"default\", \"endUser\"],\n      \"default\": \"default\"\n    },\n    \"groups\": {\n      \"type\": \"array\",\n      \"description\": \"Groups the user belongs to.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": { \"type\": \"integer\" },\n          \"name\": { \"type\": \"string\" }\n        }\n      }\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the user was created.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n   \
  \   \"description\": \"Timestamp when the user was last updated.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/retool/refs/heads/main/json-schema/retool-user-schema.json
tags:
- Admin Panel
- Dashboard
- Internal Tools
- Low Code
- No Code
title: Retool User
---
