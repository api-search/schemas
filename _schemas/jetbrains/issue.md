---
description: An issue resource in JetBrains YouTrack issue tracker.
layout: schema
name: JetBrains YouTrack Issue
properties_list:
- description: Unique entity identifier.
  name: id
  type: string
- description: Human-readable issue ID (e.g., PROJECT-123).
  name: idReadable
  type: string
- description: Short summary or title of the issue.
  name: summary
  type: string
- description: Detailed description of the issue.
  name: description
  type: string
- description: Timestamp when the issue was created (Unix ms).
  name: created
  type: integer
- description: Timestamp when the issue was last updated (Unix ms).
  name: updated
  type: integer
- description: Timestamp when the issue was resolved (Unix ms), or null.
  name: resolved
  type:
  - integer
  - 'null'
- description: User who reported the issue.
  name: reporter
  type: object
- description: Project the issue belongs to.
  name: project
  type: object
- description: Tags applied to the issue.
  name: tags
  type: array
- description: Number of comments on the issue.
  name: commentsCount
  type: integer
provider_name: JetBrains
provider_slug: jetbrains
schema_file: json-schema/issue.json
slug: issue
source_filename: issue.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"jetbrains-issue.json\",\n  \"title\": \"JetBrains YouTrack Issue\",\n  \"description\": \"An issue resource in JetBrains YouTrack issue tracker.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique entity identifier.\"\n    },\n    \"idReadable\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable issue ID (e.g., PROJECT-123).\"\n    },\n    \"summary\": {\n      \"type\": \"string\",\n      \"description\": \"Short summary or title of the issue.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Detailed description of the issue.\"\n    },\n    \"created\": {\n      \"type\": \"integer\",\n      \"description\": \"Timestamp when the issue was created (Unix ms).\"\n    },\n    \"updated\": {\n      \"type\": \"integer\",\n      \"description\": \"Timestamp when the\
  \ issue was last updated (Unix ms).\"\n    },\n    \"resolved\": {\n      \"type\": [\"integer\", \"null\"],\n      \"description\": \"Timestamp when the issue was resolved (Unix ms), or null.\"\n    },\n    \"reporter\": {\n      \"type\": \"object\",\n      \"description\": \"User who reported the issue.\",\n      \"properties\": {\n        \"id\": { \"type\": \"string\" },\n        \"login\": { \"type\": \"string\" },\n        \"fullName\": { \"type\": \"string\" }\n      }\n    },\n    \"project\": {\n      \"type\": \"object\",\n      \"description\": \"Project the issue belongs to.\",\n      \"properties\": {\n        \"id\": { \"type\": \"string\" },\n        \"name\": { \"type\": \"string\" },\n        \"shortName\": { \"type\": \"string\" }\n      }\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"Tags applied to the issue.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": { \"type\": \"string\" },\n\
  \          \"name\": { \"type\": \"string\" }\n        }\n      }\n    },\n    \"commentsCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of comments on the issue.\"\n    }\n  },\n  \"required\": [\"id\", \"summary\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/jetbrains/refs/heads/main/json-schema/issue.json
tags:
- CI/CD
- Developer Tools
- IDE
title: JetBrains YouTrack Issue
---
