---
description: Represents an organization in Sentry. Organizations are the top-level entity that contain projects, teams, and members.
layout: schema
name: Sentry Organization
properties_list:
- description: The unique identifier of the organization.
  name: id
  type: string
- description: The URL-friendly slug of the organization.
  name: slug
  type: string
- description: The human-readable name of the organization.
  name: name
  type: string
- description: When the organization was created.
  name: dateCreated
  type: string
- description: The status of the organization.
  name: status
  type: object
- description: Whether the organization opted in to early adopter features.
  name: isEarlyAdopter
  type: boolean
- description: The organization's avatar settings.
  name: avatar
  type: object
- description: A list of feature flags enabled for this organization.
  name: features
  type: array
- description: The organization's quota settings.
  name: quota
  type: object
provider_name: Sentry
provider_slug: sentry-system
schema_file: json-schema/sentry-organization-schema.json
slug: sentry-organization
source_filename: sentry-organization-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://sentry.io/schemas/organization.json\",\n  \"title\": \"Sentry Organization\",\n  \"description\": \"Represents an organization in Sentry. Organizations are the top-level entity that contain projects, teams, and members.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the organization.\"\n    },\n    \"slug\": {\n      \"type\": \"string\",\n      \"description\": \"The URL-friendly slug of the organization.\",\n      \"pattern\": \"^[a-z0-9_-]+$\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The human-readable name of the organization.\"\n    },\n    \"dateCreated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the organization was created.\"\n    },\n    \"status\": {\n      \"type\": \"object\",\n      \"\
  description\": \"The status of the organization.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"name\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"isEarlyAdopter\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the organization opted in to early adopter features.\"\n    },\n    \"avatar\": {\n      \"type\": \"object\",\n      \"description\": \"The organization's avatar settings.\",\n      \"properties\": {\n        \"avatarType\": {\n          \"type\": \"string\",\n          \"description\": \"The type of avatar (e.g., letter_avatar, upload).\"\n        },\n        \"avatarUuid\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The UUID of the uploaded avatar, if any.\"\n        }\n      }\n    },\n    \"features\": {\n      \"type\": \"array\",\n      \"description\": \"A list of feature flags enabled for this organization.\",\n      \"items\": {\n     \
  \   \"type\": \"string\"\n      }\n    },\n    \"quota\": {\n      \"type\": \"object\",\n      \"description\": \"The organization's quota settings.\",\n      \"properties\": {\n        \"maxRate\": {\n          \"type\": [\"integer\", \"null\"],\n          \"description\": \"The maximum event rate.\"\n        },\n        \"maxRateInterval\": {\n          \"type\": \"integer\",\n          \"description\": \"The interval in seconds for the max rate.\"\n        },\n        \"accountLimit\": {\n          \"type\": \"integer\",\n          \"description\": \"The account-level event limit.\"\n        },\n        \"projectLimit\": {\n          \"type\": \"integer\",\n          \"description\": \"The per-project event limit.\"\n        }\n      }\n    }\n  },\n  \"required\": [\"id\", \"slug\", \"name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sentry-system/refs/heads/main/json-schema/sentry-organization-schema.json
tags:
- APM
- Application Monitoring
- Bug Tracking
- Developer Tools
- Error Tracking
- Observability
- Performance Monitoring
- Real-Time Monitoring
title: Sentry Organization
---
