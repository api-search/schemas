---
description: SharePoint list item.
layout: schema
name: ListItem
properties_list:
- description: ''
  name: Id
  type: integer
- description: ''
  name: Title
  type: string
- description: ''
  name: Created
  type: string
- description: ''
  name: Modified
  type: string
- description: ''
  name: AuthorId
  type: integer
- description: ''
  name: EditorId
  type: integer
provider_name: Microsoft SharePoint
provider_slug: sharepoint
schema_file: json-schema/sharepoint-list-item-schema.json
slug: sharepoint-list-item
source_filename: sharepoint-list-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/sharepoint/refs/heads/main/json-schema/sharepoint-list-item-schema.json\",\n  \"title\": \"ListItem\",\n  \"description\": \"SharePoint list item.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"integer\",\n      \"example\": 1\n    },\n    \"Title\": {\n      \"type\": \"string\",\n      \"example\": \"My Task\"\n    },\n    \"Created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-04-17T09:00:00Z\"\n    },\n    \"Modified\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-04-17T10:30:00Z\"\n    },\n    \"AuthorId\": {\n      \"type\": \"integer\",\n      \"example\": 7\n    },\n    \"EditorId\": {\n      \"type\": \"integer\",\n      \"example\": 7\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sharepoint/refs/heads/main/json-schema/sharepoint-list-item-schema.json
tags:
- Collaboration
- Document Management
- Enterprise Content Management
- Intranet
- Microsoft
title: ListItem
---
