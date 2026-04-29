---
description: A tool available on a project's dock
layout: schema
name: DockItem
properties_list:
- description: Dock item ID
  name: id
  type: integer
- description: Display title of the tool
  name: title
  type: string
- description: Internal name of the tool (e.g., message_board, todoset)
  name: name
  type: string
- description: Whether this tool is enabled on the project
  name: enabled
  type: boolean
- description: Display position of the tool in the dock
  name: position
  type: integer
- description: API URL for this tool's resource
  name: url
  type: string
- description: Web URL for this tool's resource
  name: app_url
  type: string
provider_name: Basecamp
provider_slug: basecamp
schema_file: json-schema/dockitem-schema.json
slug: dockitem
source_filename: dockitem-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/basecamp/json-schema/dockitem-schema.json\",\n  \"title\": \"DockItem\",\n  \"type\": \"object\",\n  \"description\": \"A tool available on a project's dock\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Dock item ID\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Display title of the tool\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Internal name of the tool (e.g., message_board, todoset)\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this tool is enabled on the project\"\n    },\n    \"position\": {\n      \"type\": \"integer\",\n      \"description\": \"Display position of the tool in the dock\",\n      \"nullable\": true\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"\
  uri\",\n      \"description\": \"API URL for this tool's resource\"\n    },\n    \"app_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Web URL for this tool's resource\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/basecamp/refs/heads/main/json-schema/dockitem-schema.json
tags:
- Collaboration
- Project Management
- REST
- SaaS
- Team Communication
title: DockItem
---
