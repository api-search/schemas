---
description: JSON Schema for a Bluebeam Studio Session used for collaborative PDF document review and markup.
layout: schema
name: Bluebeam Studio Session
properties_list:
- description: Unique Studio Session identifier
  name: id
  type: string
- description: Session display name
  name: name
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: status
  type: string
- description: URL users can use to join the session
  name: inviteUrl
  type: string
- description: Default permission level for new attendees
  name: defaultPermission
  type: string
- description: Whether attendees can invite others
  name: allowInvitations
  type: boolean
- description: Whether the session requires explicit invitation
  name: restricted
  type: boolean
- description: User who created the session
  name: createdBy
  type: string
- description: ''
  name: createdAt
  type: string
- description: ''
  name: finishedAt
  type: string
- description: ''
  name: documentCount
  type: integer
- description: ''
  name: userCount
  type: integer
provider_name: bluebeam
provider_slug: bluebeam
schema_file: json-schema/bluebeam-session-schema.json
slug: bluebeam-session
source_filename: bluebeam-session-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bluebeam/refs/heads/main/json-schema/bluebeam-session-schema.json\",\n  \"title\": \"Bluebeam Studio Session\",\n  \"description\": \"JSON Schema for a Bluebeam Studio Session used for collaborative PDF document review and markup.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\", \"status\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique Studio Session identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Session display name\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"Active\", \"Finished\", \"Pending\"]\n    },\n    \"inviteUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL users can use to join the session\"\
  \n    },\n    \"defaultPermission\": {\n      \"type\": \"string\",\n      \"enum\": [\"ReadOnly\", \"MarkupOnly\", \"FullAccess\"],\n      \"description\": \"Default permission level for new attendees\"\n    },\n    \"allowInvitations\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether attendees can invite others\"\n    },\n    \"restricted\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the session requires explicit invitation\"\n    },\n    \"createdBy\": {\n      \"type\": \"string\",\n      \"description\": \"User who created the session\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"finishedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"documentCount\": {\n      \"type\": \"integer\",\n      \"minimum\": 0\n    },\n    \"userCount\": {\n      \"type\": \"integer\",\n      \"minimum\": 0\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bluebeam/refs/heads/main/json-schema/bluebeam-session-schema.json
tags: []
title: Bluebeam Studio Session
---
