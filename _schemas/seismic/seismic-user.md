---
description: A user account in the Seismic platform with associated profile information, role, and team membership.
layout: schema
name: Seismic User
properties_list:
- description: Unique identifier of the user.
  name: id
  type: string
- description: Email address of the user.
  name: email
  type: string
- description: First name of the user.
  name: firstName
  type: string
- description: Last name of the user.
  name: lastName
  type: string
- description: Display name of the user.
  name: displayName
  type: string
- description: Job title of the user.
  name: title
  type: string
- description: Department the user belongs to.
  name: department
  type: string
- description: ID of the assigned role.
  name: roleId
  type: string
- description: Name of the assigned role.
  name: roleName
  type: string
- description: ID of the team the user belongs to.
  name: teamId
  type: string
- description: Name of the team the user belongs to.
  name: teamName
  type: string
- description: Account status of the user.
  name: status
  type: string
- description: URL of the user's avatar image.
  name: avatarUrl
  type: string
- description: Timestamp of the user's last login.
  name: lastLoginAt
  type:
  - string
  - 'null'
- description: Timestamp when the user account was created.
  name: createdAt
  type: string
- description: Timestamp when the user account was last modified.
  name: modifiedAt
  type: string
provider_name: Seismic
provider_slug: seismic
schema_file: json-schema/seismic-user-schema.json
slug: seismic-user
source_filename: seismic-user-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.seismic.com/schemas/user\",\n  \"title\": \"Seismic User\",\n  \"description\": \"A user account in the Seismic platform with associated profile information, role, and team membership.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the user.\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Email address of the user.\"\n    },\n    \"firstName\": {\n      \"type\": \"string\",\n      \"description\": \"First name of the user.\"\n    },\n    \"lastName\": {\n      \"type\": \"string\",\n      \"description\": \"Last name of the user.\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the user.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Job title of the user.\"\n    },\n    \"department\": {\n      \"type\": \"string\",\n      \"description\": \"Department the user belongs to.\"\n    },\n    \"roleId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the assigned role.\"\n    },\n    \"roleName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the assigned role.\"\n    },\n    \"teamId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the team the user belongs to.\"\n    },\n    \"teamName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the team the user belongs to.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Account status of the user.\",\n      \"enum\": [\"active\", \"inactive\", \"pending\", \"suspended\"]\n    },\n    \"avatarUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the user's avatar image.\"\n    },\n    \"lastLoginAt\": {\n      \"type\": [\"\
  string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of the user's last login.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the user account was created.\"\n    },\n    \"modifiedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the user account was last modified.\"\n    }\n  },\n  \"required\": [\"id\", \"email\", \"firstName\", \"lastName\"]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/seismic/refs/heads/main/json-schema/seismic-user-schema.json
tags: []
title: Seismic User
---
