---
description: Represents an issue (group) in Sentry. Issues are aggregated groups of similar error events, providing a deduplicated view of recurring problems in an application.
layout: schema
name: Sentry Issue
properties_list:
- description: The unique identifier of the issue.
  name: id
  type: string
- description: The short ID for the issue (e.g., PROJECT-123), used in the Sentry UI.
  name: shortId
  type: string
- description: The title of the issue, typically the error type and message.
  name: title
  type: string
- description: The function or module where the issue originated.
  name: culprit
  type: string
- description: The permanent URL to view this issue in the Sentry UI.
  name: permalink
  type: string
- description: The severity level of the issue.
  name: level
  type: string
- description: The current status of the issue.
  name: status
  type: string
- description: The platform that generated the issue.
  name: platform
  type: string
- description: When the issue was first seen.
  name: firstSeen
  type: string
- description: When the issue was most recently seen.
  name: lastSeen
  type: string
- description: The total number of events for this issue.
  name: count
  type: string
- description: The number of unique users affected by this issue.
  name: userCount
  type: integer
- description: The type of issue.
  name: type
  type: string
- description: Additional metadata about the issue.
  name: metadata
  type: object
- description: The user or team assigned to this issue.
  name: assignedTo
  type:
  - object
  - 'null'
- description: Whether the issue is publicly visible.
  name: isPublic
  type: boolean
- description: Whether the authenticated user has seen this issue.
  name: hasSeen
  type: boolean
- description: Whether the issue is bookmarked by the authenticated user.
  name: isBookmarked
  type: boolean
- description: The project this issue belongs to.
  name: project
  type: object
provider_name: Sentry
provider_slug: sentry-system
schema_file: json-schema/sentry-issue-schema.json
slug: sentry-issue
source_filename: sentry-issue-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://sentry.io/schemas/issue.json\",\n  \"title\": \"Sentry Issue\",\n  \"description\": \"Represents an issue (group) in Sentry. Issues are aggregated groups of similar error events, providing a deduplicated view of recurring problems in an application.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the issue.\"\n    },\n    \"shortId\": {\n      \"type\": \"string\",\n      \"description\": \"The short ID for the issue (e.g., PROJECT-123), used in the Sentry UI.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The title of the issue, typically the error type and message.\"\n    },\n    \"culprit\": {\n      \"type\": \"string\",\n      \"description\": \"The function or module where the issue originated.\"\n    },\n    \"permalink\": {\n      \"type\": \"string\"\
  ,\n      \"format\": \"uri\",\n      \"description\": \"The permanent URL to view this issue in the Sentry UI.\"\n    },\n    \"level\": {\n      \"type\": \"string\",\n      \"description\": \"The severity level of the issue.\",\n      \"enum\": [\"fatal\", \"error\", \"warning\", \"info\", \"debug\"]\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the issue.\",\n      \"enum\": [\"resolved\", \"unresolved\", \"ignored\"]\n    },\n    \"platform\": {\n      \"type\": \"string\",\n      \"description\": \"The platform that generated the issue.\"\n    },\n    \"firstSeen\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the issue was first seen.\"\n    },\n    \"lastSeen\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the issue was most recently seen.\"\n    },\n    \"count\": {\n      \"type\": \"string\",\n      \"description\": \"\
  The total number of events for this issue.\"\n    },\n    \"userCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of unique users affected by this issue.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of issue.\",\n      \"enum\": [\"error\", \"default\"]\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"description\": \"Additional metadata about the issue.\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"The error type (e.g., ValueError, TypeError).\"\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"description\": \"The error message or value.\"\n        },\n        \"filename\": {\n          \"type\": \"string\",\n          \"description\": \"The filename where the error occurred.\"\n        },\n        \"function\": {\n          \"type\": \"string\",\n          \"description\": \"The function where the\
  \ error occurred.\"\n        }\n      }\n    },\n    \"assignedTo\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"The user or team assigned to this issue.\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\"user\", \"team\"]\n        },\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"name\": {\n          \"type\": \"string\"\n        },\n        \"email\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"isPublic\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the issue is publicly visible.\"\n    },\n    \"hasSeen\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the authenticated user has seen this issue.\"\n    },\n    \"isBookmarked\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the issue is bookmarked by the authenticated user.\"\n    },\n    \"project\": {\n      \"type\": \"object\",\n      \"description\"\
  : \"The project this issue belongs to.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"slug\": {\n          \"type\": \"string\"\n        },\n        \"name\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  },\n  \"required\": [\"id\", \"title\", \"status\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sentry-system/refs/heads/main/json-schema/sentry-issue-schema.json
tags:
- APM
- Application Monitoring
- Bug Tracking
- Developer Tools
- Error Tracking
- Observability
- Performance Monitoring
- Real-Time Monitoring
title: Sentry Issue
---
