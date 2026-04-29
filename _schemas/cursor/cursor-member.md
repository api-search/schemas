---
description: Schema for a team member returned by the Cursor Admin API.
layout: schema
name: Cursor Team Member
properties_list:
- description: Unique identifier for the team member.
  name: id
  type: string
- description: Member's email address.
  name: email
  type: string
- description: Display name of the member.
  name: name
  type: string
- description: Role assigned to the member within the team.
  name: role
  type: string
- description: Whether the member has been removed from the team.
  name: isRemoved
  type: boolean
provider_name: Cursor
provider_slug: cursor
schema_file: json-schema/cursor-member-schema.json
slug: cursor-member
source_filename: cursor-member-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/cursor/refs/heads/main/json-schema/cursor-member-schema.json\",\n  \"title\": \"Cursor Team Member\",\n  \"description\": \"Schema for a team member returned by the Cursor Admin API.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"email\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the team member.\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Member's email address.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the member.\"\n    },\n    \"role\": {\n      \"type\": \"string\",\n      \"enum\": [\"member\", \"admin\", \"owner\"],\n      \"description\": \"Role assigned to the member within the team.\"\n    },\n    \"isRemoved\": {\n      \"type\": \"\
  boolean\",\n      \"description\": \"Whether the member has been removed from the team.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cursor/refs/heads/main/json-schema/cursor-member-schema.json
tags:
- AI
- AI Editor
- Code Generation
- Coding Assistant
- Copilot
- Developer Tools
- LLM
- Productivity
- VSCode Fork
title: Cursor Team Member
---
