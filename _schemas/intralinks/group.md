---
description: A group within an Intralinks workspace that organizes users and controls document access permissions. Permissions in Intralinks are assigned at the group level.
layout: schema
name: Intralinks Group
properties_list:
- description: Unique identifier of the group.
  name: id
  type: string
- description: Group name.
  name: name
  type: string
- description: Group type.
  name: type
  type: string
- description: Group description or note.
  name: note
  type: string
- description: Number of members in the group.
  name: memberCount
  type: integer
- description: Number of folders accessible to this group.
  name: foldersWithAccess
  type: integer
- description: Group creation timestamp.
  name: createdOn
  type: string
- description: Last modification timestamp.
  name: updatedOn
  type: string
provider_name: Intralinks
provider_slug: intralinks
schema_file: json-schema/group.json
slug: group
source_filename: group.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"group.json\",\n  \"title\": \"Intralinks Group\",\n  \"description\": \"A group within an Intralinks workspace that organizes users and controls document access permissions. Permissions in Intralinks are assigned at the group level.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the group.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Group name.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Group type.\"\n    },\n    \"note\": {\n      \"type\": \"string\",\n      \"description\": \"Group description or note.\"\n    },\n    \"memberCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of members in the group.\"\n    },\n    \"foldersWithAccess\": {\n      \"type\": \"integer\",\n      \"description\": \"Number\
  \ of folders accessible to this group.\"\n    },\n    \"createdOn\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Group creation timestamp.\"\n    },\n    \"updatedOn\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Last modification timestamp.\"\n    }\n  },\n  \"required\": [\"name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/intralinks/refs/heads/main/json-schema/group.json
tags:
- Document Management
- Secure File Sharing
- Virtual Data Room
title: Intralinks Group
---
