---
description: Represents a project in Sentry. Projects belong to an organization and a team, and contain issues and events for a specific application or service.
layout: schema
name: Sentry Project
properties_list:
- description: The unique identifier of the project.
  name: id
  type: string
- description: The URL-friendly slug of the project.
  name: slug
  type: string
- description: The human-readable name of the project.
  name: name
  type: string
- description: The platform identifier (e.g., python, javascript, react-native).
  name: platform
  type:
  - string
  - 'null'
- description: When the project was created.
  name: dateCreated
  type: string
- description: Whether the project is bookmarked by the authenticated user.
  name: isBookmarked
  type: boolean
- description: Whether the authenticated user is a member of this project.
  name: isMember
  type: boolean
- description: A list of feature flags enabled for this project.
  name: features
  type: array
- description: The timestamp of the first event received for this project.
  name: firstEvent
  type:
  - string
  - 'null'
- description: Whether the project has received a transaction event.
  name: firstTransactionEvent
  type: boolean
- description: Whether the authenticated user has access to this project.
  name: hasAccess
  type: boolean
- description: The primary team associated with this project.
  name: team
  type: object
- description: All teams that have access to this project.
  name: teams
  type: array
- description: The organization this project belongs to.
  name: organization
  type: object
provider_name: Sentry
provider_slug: sentry-system
schema_file: json-schema/sentry-project-schema.json
slug: sentry-project
source_filename: sentry-project-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://sentry.io/schemas/project.json\",\n  \"title\": \"Sentry Project\",\n  \"description\": \"Represents a project in Sentry. Projects belong to an organization and a team, and contain issues and events for a specific application or service.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the project.\"\n    },\n    \"slug\": {\n      \"type\": \"string\",\n      \"description\": \"The URL-friendly slug of the project.\",\n      \"pattern\": \"^[a-z0-9_-]+$\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The human-readable name of the project.\"\n    },\n    \"platform\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The platform identifier (e.g., python, javascript, react-native).\"\n    },\n    \"dateCreated\": {\n      \"type\": \"string\"\
  ,\n      \"format\": \"date-time\",\n      \"description\": \"When the project was created.\"\n    },\n    \"isBookmarked\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the project is bookmarked by the authenticated user.\"\n    },\n    \"isMember\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the authenticated user is a member of this project.\"\n    },\n    \"features\": {\n      \"type\": \"array\",\n      \"description\": \"A list of feature flags enabled for this project.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"firstEvent\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp of the first event received for this project.\"\n    },\n    \"firstTransactionEvent\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the project has received a transaction event.\"\n    },\n    \"hasAccess\": {\n      \"type\": \"boolean\",\n  \
  \    \"description\": \"Whether the authenticated user has access to this project.\"\n    },\n    \"team\": {\n      \"type\": \"object\",\n      \"description\": \"The primary team associated with this project.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"slug\": {\n          \"type\": \"string\"\n        },\n        \"name\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"teams\": {\n      \"type\": \"array\",\n      \"description\": \"All teams that have access to this project.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\"\n          },\n          \"slug\": {\n            \"type\": \"string\"\n          },\n          \"name\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"organization\": {\n      \"type\": \"object\",\n      \"description\": \"The organization this project belongs\
  \ to.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"slug\": {\n          \"type\": \"string\"\n        },\n        \"name\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  },\n  \"required\": [\"id\", \"slug\", \"name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sentry-system/refs/heads/main/json-schema/sentry-project-schema.json
tags:
- APM
- Application Monitoring
- Bug Tracking
- Developer Tools
- Error Tracking
- Observability
- Performance Monitoring
- Real-Time Monitoring
title: Sentry Project
---
