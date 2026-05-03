---
description: Represents a release in Sentry. Releases track deployments of application versions and link error events to specific code changes, commits, and deployment environments.
layout: schema
name: Sentry Release
properties_list:
- description: The internal unique identifier of the release.
  name: id
  type: integer
- description: The version identifier of the release, unique within the organization.
  name: version
  type: string
- description: A shortened version string for display purposes.
  name: shortVersion
  type: string
- description: An optional commit reference (SHA).
  name: ref
  type:
  - string
  - 'null'
- description: A URL pointing to the release (often a CI build URL).
  name: url
  type:
  - string
  - 'null'
- description: When the release was created.
  name: dateCreated
  type: string
- description: When the release went live.
  name: dateReleased
  type:
  - string
  - 'null'
- description: Timestamp of the first event for this release.
  name: firstEvent
  type:
  - string
  - 'null'
- description: Timestamp of the last event for this release.
  name: lastEvent
  type:
  - string
  - 'null'
- description: The count of new issues introduced by this release.
  name: newGroups
  type: integer
- description: Projects associated with this release.
  name: projects
  type: array
- description: Authors of commits in this release.
  name: authors
  type: array
- description: The number of commits associated with this release.
  name: commitCount
  type: integer
- description: The most recent deployment of this release.
  name: lastDeploy
  type:
  - object
  - 'null'
provider_name: Sentry
provider_slug: sentry-system
schema_file: json-schema/sentry-release-schema.json
slug: sentry-release
source_filename: sentry-release-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://sentry.io/schemas/release.json\",\n  \"title\": \"Sentry Release\",\n  \"description\": \"Represents a release in Sentry. Releases track deployments of application versions and link error events to specific code changes, commits, and deployment environments.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"The internal unique identifier of the release.\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"The version identifier of the release, unique within the organization.\"\n    },\n    \"shortVersion\": {\n      \"type\": \"string\",\n      \"description\": \"A shortened version string for display purposes.\"\n    },\n    \"ref\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"An optional commit reference (SHA).\"\n    },\n    \"url\": {\n      \"type\": [\"string\"\
  , \"null\"],\n      \"description\": \"A URL pointing to the release (often a CI build URL).\"\n    },\n    \"dateCreated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the release was created.\"\n    },\n    \"dateReleased\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"When the release went live.\"\n    },\n    \"firstEvent\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of the first event for this release.\"\n    },\n    \"lastEvent\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of the last event for this release.\"\n    },\n    \"newGroups\": {\n      \"type\": \"integer\",\n      \"description\": \"The count of new issues introduced by this release.\"\n    },\n    \"projects\": {\n      \"type\": \"array\",\n      \"description\": \"Projects\
  \ associated with this release.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"integer\"\n          },\n          \"slug\": {\n            \"type\": \"string\"\n          },\n          \"name\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"authors\": {\n      \"type\": \"array\",\n      \"description\": \"Authors of commits in this release.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\"\n          },\n          \"email\": {\n            \"type\": \"string\",\n            \"format\": \"email\"\n          }\n        }\n      }\n    },\n    \"commitCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of commits associated with this release.\"\n    },\n    \"lastDeploy\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"The most recent deployment\
  \ of this release.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"environment\": {\n          \"type\": \"string\"\n        },\n        \"dateFinished\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"date-time\"\n        }\n      }\n    }\n  },\n  \"required\": [\"version\", \"dateCreated\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sentry-system/refs/heads/main/json-schema/sentry-release-schema.json
tags:
- APM
- Application Monitoring
- Bug Tracking
- Developer Tools
- Error Tracking
- Observability
- Performance Monitoring
- Real-Time Monitoring
title: Sentry Release
---
