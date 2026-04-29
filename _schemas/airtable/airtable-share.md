---
description: A share link that provides external access to an Airtable base, view, or form. Share links can be enabled or disabled and optionally protected with a password.
layout: schema
name: Airtable Share
properties_list:
- description: The unique identifier for the share link (starts with 'shr').
  name: shareId
  type: string
- description: The type of resource being shared.
  name: type
  type: string
- description: The current state of the share link.
  name: state
  type: string
- description: The ID of the user who created the share link.
  name: createdByUserId
  type: string
- description: The time when the share link was created.
  name: createdTime
  type: string
- description: The ID of the base this share link provides access to.
  name: baseId
  type: string
- description: The ID of the specific view this share link provides access to. Null for base-level shares.
  name: viewId
  type:
  - string
  - 'null'
- description: Whether the share link requires a password to access.
  name: isPasswordEnabled
  type: boolean
- description: The effective permission level granted to anyone accessing through this share link.
  name: effectivePermissionLevel
  type: string
provider_name: Airtable
provider_slug: airtable
schema_file: json-schema/airtable-share-schema.json
slug: airtable-share
source_filename: airtable-share-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemas.airtable.com/share.json\",\n  \"title\": \"Airtable Share\",\n  \"description\": \"A share link that provides external access to an Airtable base, view, or form. Share links can be enabled or disabled and optionally protected with a password.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"shareId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the share link (starts with 'shr').\",\n      \"pattern\": \"^shr[a-zA-Z0-9]+$\",\n      \"examples\": [\"shrABC123def456\"]\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of resource being shared.\",\n      \"enum\": [\"view\", \"base\", \"form\"]\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"The current state of the share link.\",\n      \"enum\": [\"enabled\", \"disabled\"]\n    },\n    \"createdByUserId\": {\n  \
  \    \"type\": \"string\",\n      \"description\": \"The ID of the user who created the share link.\"\n    },\n    \"createdTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time when the share link was created.\"\n    },\n    \"baseId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the base this share link provides access to.\"\n    },\n    \"viewId\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The ID of the specific view this share link provides access to. Null for base-level shares.\"\n    },\n    \"isPasswordEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the share link requires a password to access.\"\n    },\n    \"effectivePermissionLevel\": {\n      \"type\": \"string\",\n      \"description\": \"The effective permission level granted to anyone accessing through this share link.\",\n      \"enum\": [\"read\", \"comment\", \"edit\"]\n    }\n  },\n  \"\
  required\": [\"shareId\", \"type\", \"state\"],\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airtable/refs/heads/main/json-schema/airtable-share-schema.json
tags:
- Applications
- Collaboration
- Data
- Databases
- Low-Code
- Productivity
- Spreadsheets
title: Airtable Share
---
