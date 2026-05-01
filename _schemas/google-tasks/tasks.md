---
description: A task resource from the Google Tasks API.
layout: schema
name: Google Task
properties_list:
- description: ''
  name: kind
  type: string
- description: Task identifier.
  name: id
  type: string
- description: ETag of the resource.
  name: etag
  type: string
- description: Title of the task.
  name: title
  type: string
- description: Last modification time of the task.
  name: updated
  type: string
- description: URL pointing to this task.
  name: selfLink
  type: string
- description: Parent task identifier.
  name: parent
  type: string
- description: String indicating the position of the task among its sibling tasks.
  name: position
  type: string
- description: Notes describing the task.
  name: notes
  type: string
- description: Status of the task.
  name: status
  type: string
- description: Due date of the task.
  name: due
  type: string
- description: Completion date of the task.
  name: completed
  type: string
- description: Flag indicating whether the task has been deleted.
  name: deleted
  type: boolean
- description: Flag indicating whether the task is hidden.
  name: hidden
  type: boolean
- description: Collection of links related to this task.
  name: links
  type: array
provider_name: Google Tasks
provider_slug: google-tasks
schema_file: json-schema/tasks.json
slug: tasks
source_filename: tasks.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/google-tasks/refs/heads/main/json-schema/tasks.json\",\n  \"title\": \"Google Task\",\n  \"description\": \"A task resource from the Google Tasks API.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"kind\": {\n      \"type\": \"string\",\n      \"const\": \"tasks#task\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Task identifier.\"\n    },\n    \"etag\": {\n      \"type\": \"string\",\n      \"description\": \"ETag of the resource.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Title of the task.\"\n    },\n    \"updated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Last modification time of the task.\"\n    },\n    \"selfLink\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL pointing\
  \ to this task.\"\n    },\n    \"parent\": {\n      \"type\": \"string\",\n      \"description\": \"Parent task identifier.\"\n    },\n    \"position\": {\n      \"type\": \"string\",\n      \"description\": \"String indicating the position of the task among its sibling tasks.\"\n    },\n    \"notes\": {\n      \"type\": \"string\",\n      \"description\": \"Notes describing the task.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"needsAction\", \"completed\"],\n      \"description\": \"Status of the task.\"\n    },\n    \"due\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Due date of the task.\"\n    },\n    \"completed\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Completion date of the task.\"\n    },\n    \"deleted\": {\n      \"type\": \"boolean\",\n      \"description\": \"Flag indicating whether the task has been deleted.\"\n    },\n    \"hidden\": {\n  \
  \    \"type\": \"boolean\",\n      \"description\": \"Flag indicating whether the task is hidden.\"\n    },\n    \"links\": {\n      \"type\": \"array\",\n      \"description\": \"Collection of links related to this task.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"type\": {\n            \"type\": \"string\"\n          },\n          \"description\": {\n            \"type\": \"string\"\n          },\n          \"link\": {\n            \"type\": \"string\",\n            \"format\": \"uri\"\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\"kind\", \"id\", \"title\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-tasks/refs/heads/main/json-schema/tasks.json
tags:
- Google
- Productivity
- Task Management
- Tasks
- Todo
- Workspace
title: Google Task
---
