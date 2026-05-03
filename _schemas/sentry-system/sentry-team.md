---
description: Represents a team in Sentry. Teams belong to an organization and are used to manage access to projects and assign ownership of issues.
layout: schema
name: Sentry Team
properties_list:
- description: The unique identifier of the team.
  name: id
  type: string
- description: The URL-friendly slug of the team.
  name: slug
  type: string
- description: The human-readable name of the team.
  name: name
  type: string
- description: When the team was created.
  name: dateCreated
  type: string
- description: Whether the authenticated user is a member of this team.
  name: isMember
  type: boolean
- description: The number of members in this team.
  name: memberCount
  type: integer
- description: The team's avatar settings.
  name: avatar
  type: object
- description: The organization this team belongs to.
  name: organization
  type: object
- description: Projects associated with this team.
  name: projects
  type: array
provider_name: Sentry
provider_slug: sentry-system
schema_file: json-schema/sentry-team-schema.json
slug: sentry-team
source_filename: sentry-team-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://sentry.io/schemas/team.json\",\n  \"title\": \"Sentry Team\",\n  \"description\": \"Represents a team in Sentry. Teams belong to an organization and are used to manage access to projects and assign ownership of issues.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the team.\"\n    },\n    \"slug\": {\n      \"type\": \"string\",\n      \"description\": \"The URL-friendly slug of the team.\",\n      \"pattern\": \"^[a-z0-9_-]+$\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The human-readable name of the team.\"\n    },\n    \"dateCreated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the team was created.\"\n    },\n    \"isMember\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the authenticated\
  \ user is a member of this team.\"\n    },\n    \"memberCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of members in this team.\"\n    },\n    \"avatar\": {\n      \"type\": \"object\",\n      \"description\": \"The team's avatar settings.\",\n      \"properties\": {\n        \"avatarType\": {\n          \"type\": \"string\"\n        },\n        \"avatarUuid\": {\n          \"type\": [\"string\", \"null\"]\n        }\n      }\n    },\n    \"organization\": {\n      \"type\": \"object\",\n      \"description\": \"The organization this team belongs to.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"slug\": {\n          \"type\": \"string\"\n        },\n        \"name\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"projects\": {\n      \"type\": \"array\",\n      \"description\": \"Projects associated with this team.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"\
  properties\": {\n          \"id\": {\n            \"type\": \"string\"\n          },\n          \"slug\": {\n            \"type\": \"string\"\n          },\n          \"name\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\"id\", \"slug\", \"name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sentry-system/refs/heads/main/json-schema/sentry-team-schema.json
tags:
- APM
- Application Monitoring
- Bug Tracking
- Developer Tools
- Error Tracking
- Observability
- Performance Monitoring
- Real-Time Monitoring
title: Sentry Team
---
