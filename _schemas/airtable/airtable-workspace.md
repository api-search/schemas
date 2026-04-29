---
description: An Airtable workspace is an organizational container that groups related bases together. Workspaces provide a shared collaboration boundary with configurable permissions for team members.
layout: schema
name: Airtable Workspace
properties_list:
- description: The unique identifier for the workspace (starts with 'wsp').
  name: id
  type: string
- description: The display name of the workspace.
  name: name
  type: string
- description: The individual user collaborators on this workspace.
  name: collaborators
  type: array
- description: The user group collaborators on this workspace.
  name: groupCollaborators
  type: array
provider_name: Airtable
provider_slug: airtable
schema_file: json-schema/airtable-workspace-schema.json
slug: airtable-workspace
source_filename: airtable-workspace-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemas.airtable.com/workspace.json\",\n  \"title\": \"Airtable Workspace\",\n  \"description\": \"An Airtable workspace is an organizational container that groups related bases together. Workspaces provide a shared collaboration boundary with configurable permissions for team members.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the workspace (starts with 'wsp').\",\n      \"pattern\": \"^wsp[a-zA-Z0-9]+$\",\n      \"examples\": [\"wspABC123def456\"]\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the workspace.\"\n    },\n    \"collaborators\": {\n      \"type\": \"array\",\n      \"description\": \"The individual user collaborators on this workspace.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n \
  \         \"userId\": {\n            \"type\": \"string\",\n            \"description\": \"The unique identifier of the collaborator.\"\n          },\n          \"email\": {\n            \"type\": \"string\",\n            \"format\": \"email\",\n            \"description\": \"The email address of the collaborator.\"\n          },\n          \"permissionLevel\": {\n            \"type\": \"string\",\n            \"description\": \"The permission level of the collaborator.\",\n            \"enum\": [\"owner\", \"creator\", \"editor\", \"commenter\", \"read\"]\n          }\n        },\n        \"required\": [\"userId\", \"permissionLevel\"]\n      }\n    },\n    \"groupCollaborators\": {\n      \"type\": \"array\",\n      \"description\": \"The user group collaborators on this workspace.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"groupId\": {\n            \"type\": \"string\",\n            \"description\": \"The unique identifier of the user\
  \ group.\"\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"The name of the user group.\"\n          },\n          \"permissionLevel\": {\n            \"type\": \"string\",\n            \"description\": \"The permission level of the group.\",\n            \"enum\": [\"owner\", \"creator\", \"editor\", \"commenter\", \"read\"]\n          }\n        },\n        \"required\": [\"groupId\", \"permissionLevel\"]\n      }\n    }\n  },\n  \"required\": [\"id\", \"name\"],\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airtable/refs/heads/main/json-schema/airtable-workspace-schema.json
tags:
- Applications
- Collaboration
- Data
- Databases
- Low-Code
- Productivity
- Spreadsheets
title: Airtable Workspace
---
