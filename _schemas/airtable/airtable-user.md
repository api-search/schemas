---
description: An Airtable user account within an enterprise organization. Users have identity attributes, management states, and permission levels across workspaces and bases.
layout: schema
name: Airtable User
properties_list:
- description: The unique identifier for the user (starts with 'usr').
  name: id
  type: string
- description: The email address of the user.
  name: email
  type: string
- description: The display name of the user.
  name: name
  type: string
- description: The management state of the user within the enterprise.
  name: state
  type: string
- description: Whether the user has enterprise administrator privileges.
  name: isAdmin
  type: boolean
- description: The time when the user account was created.
  name: createdTime
  type: string
- description: The time of the user's most recent activity. Null if the user has never been active.
  name: lastActivityTime
  type:
  - string
  - 'null'
- description: The user's collaboration details across workspaces, bases, and interfaces.
  name: collaborations
  type: object
provider_name: Airtable
provider_slug: airtable
schema_file: json-schema/airtable-user-schema.json
slug: airtable-user
source_filename: airtable-user-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemas.airtable.com/user.json\",\n  \"title\": \"Airtable User\",\n  \"description\": \"An Airtable user account within an enterprise organization. Users have identity attributes, management states, and permission levels across workspaces and bases.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the user (starts with 'usr').\",\n      \"pattern\": \"^usr[a-zA-Z0-9]+$\",\n      \"examples\": [\"usrABC123def456\"]\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"The email address of the user.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the user.\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"The management state of the user within the enterprise.\"\
  ,\n      \"enum\": [\"managed\", \"unmanaged\", \"deactivated\"]\n    },\n    \"isAdmin\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user has enterprise administrator privileges.\"\n    },\n    \"createdTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time when the user account was created.\"\n    },\n    \"lastActivityTime\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"The time of the user's most recent activity. Null if the user has never been active.\"\n    },\n    \"collaborations\": {\n      \"type\": \"object\",\n      \"description\": \"The user's collaboration details across workspaces, bases, and interfaces.\",\n      \"properties\": {\n        \"workspaceCollaborations\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"workspaceId\": {\n        \
  \        \"type\": \"string\"\n              },\n              \"permissionLevel\": {\n                \"type\": \"string\",\n                \"enum\": [\"owner\", \"creator\", \"editor\", \"commenter\", \"read\"]\n              }\n            }\n          }\n        },\n        \"baseCollaborations\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"baseId\": {\n                \"type\": \"string\"\n              },\n              \"permissionLevel\": {\n                \"type\": \"string\",\n                \"enum\": [\"owner\", \"creator\", \"editor\", \"commenter\", \"read\"]\n              }\n            }\n          }\n        },\n        \"interfaceCollaborations\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"baseId\": {\n                \"type\": \"string\"\n              },\n              \"\
  interfaceId\": {\n                \"type\": \"string\"\n              },\n              \"permissionLevel\": {\n                \"type\": \"string\"\n              }\n            }\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\"id\", \"email\", \"state\"],\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airtable/refs/heads/main/json-schema/airtable-user-schema.json
tags:
- Applications
- Collaboration
- Data
- Databases
- Low-Code
- Productivity
- Spreadsheets
title: Airtable User
---
