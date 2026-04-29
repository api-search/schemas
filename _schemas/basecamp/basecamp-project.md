---
description: Represents a Basecamp project (bucket), which is the top-level container for all collaboration content including messages, to-dos, documents, schedules, campfires, and card tables. Projects are owned by an account and can be accessed by invited team members and clients.
layout: schema
name: Basecamp Project
properties_list:
- description: Unique identifier for the project within the Basecamp account
  name: id
  type: integer
- description: Current lifecycle status of the project
  name: status
  type: string
- description: ISO 8601 UTC timestamp when the project was created
  name: created_at
  type: string
- description: ISO 8601 UTC timestamp when the project was last updated
  name: updated_at
  type: string
- description: Human-readable name of the project
  name: name
  type: string
- description: Optional description providing context about the project's purpose or scope
  name: description
  type:
  - string
  - 'null'
- description: Project purpose classification such as 'team_project' or 'company_hq'
  name: purpose
  type: string
- description: Whether client visibility is enabled for this project, allowing invited client users to view designated content
  name: clients_enabled
  type: boolean
- description: Whether timesheet tracking is enabled for this project
  name: timesheet_enabled
  type: boolean
- description: Optional color identifier used to visually distinguish the project in the Basecamp interface
  name: color
  type:
  - string
  - 'null'
- description: Canonical API URL for this project resource
  name: url
  type: string
- description: Web URL to open this project in the Basecamp application
  name: app_url
  type: string
- description: API URL to bookmark this project for the authenticated user
  name: bookmark_url
  type: string
- description: List of tools available on this project's dock, each representing an enabled feature such as messages, to-dos, schedule, or campfire
  name: dock
  type: array
provider_name: Basecamp
provider_slug: basecamp
schema_file: json-schema/basecamp-project-schema.json
slug: basecamp-project
source_filename: basecamp-project-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/basecamp/bc3-api/schemas/basecamp/project.json\",\n  \"title\": \"Basecamp Project\",\n  \"description\": \"Represents a Basecamp project (bucket), which is the top-level container for all collaboration content including messages, to-dos, documents, schedules, campfires, and card tables. Projects are owned by an account and can be accessed by invited team members and clients.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\", \"status\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique identifier for the project within the Basecamp account\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current lifecycle status of the project\",\n      \"enum\": [\"active\", \"archived\", \"trashed\"]\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\
  ,\n      \"description\": \"ISO 8601 UTC timestamp when the project was created\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 UTC timestamp when the project was last updated\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable name of the project\",\n      \"minLength\": 1,\n      \"maxLength\": 255\n    },\n    \"description\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Optional description providing context about the project's purpose or scope\"\n    },\n    \"purpose\": {\n      \"type\": \"string\",\n      \"description\": \"Project purpose classification such as 'team_project' or 'company_hq'\"\n    },\n    \"clients_enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether client visibility is enabled for this project, allowing invited client users to view designated content\"\n    },\n    \"timesheet_enabled\"\
  : {\n      \"type\": \"boolean\",\n      \"description\": \"Whether timesheet tracking is enabled for this project\"\n    },\n    \"color\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Optional color identifier used to visually distinguish the project in the Basecamp interface\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Canonical API URL for this project resource\"\n    },\n    \"app_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Web URL to open this project in the Basecamp application\"\n    },\n    \"bookmark_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"API URL to bookmark this project for the authenticated user\"\n    },\n    \"dock\": {\n      \"type\": \"array\",\n      \"description\": \"List of tools available on this project's dock, each representing an enabled feature such as messages, to-dos, schedule,\
  \ or campfire\",\n      \"items\": {\n        \"$ref\": \"#/$defs/DockItem\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"DockItem\": {\n      \"type\": \"object\",\n      \"description\": \"A tool or feature available on a Basecamp project dock\",\n      \"required\": [\"id\", \"title\", \"name\", \"enabled\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\",\n          \"description\": \"Unique identifier for this dock item resource\"\n        },\n        \"title\": {\n          \"type\": \"string\",\n          \"description\": \"Display title of the tool shown to users (e.g., 'Message Board', 'To-dos')\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Internal machine-readable name of the tool\",\n          \"enum\": [\n            \"message_board\",\n            \"todoset\",\n            \"vault\",\n            \"schedule\",\n            \"inbox\",\n            \"chat\",\n            \"questionnaire\",\n \
  \           \"kanban_board\"\n          ]\n        },\n        \"enabled\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether this tool is currently enabled and visible on the project\"\n        },\n        \"position\": {\n          \"type\": [\"integer\", \"null\"],\n          \"description\": \"Display order position of this tool in the project dock\"\n        },\n        \"url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"API URL for this tool's resource within the project\"\n        },\n        \"app_url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"Web URL to open this tool within the project in the Basecamp application\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/basecamp/refs/heads/main/json-schema/basecamp-project-schema.json
tags:
- Collaboration
- Project Management
- REST
- SaaS
- Team Communication
title: Basecamp Project
---
