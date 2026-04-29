---
description: A group from an integrated directory service.
layout: schema
name: Group
properties_list:
- description: Unique identifier for the group.
  name: id
  type: string
- description: Display name of the group.
  name: name
  type: string
- description: Email address of the group.
  name: email
  type: string
- description: Description of the group.
  name: description
  type: string
- description: Number of members in the group.
  name: member_count
  type: integer
- description: When the group was created.
  name: created_at
  type: string
- description: When the group was last updated.
  name: updated_at
  type: string
provider_name: BetterCloud
provider_slug: bettercloud
schema_file: json-schema/bettercloud-group-schema.json
slug: bettercloud-group
source_filename: bettercloud-group-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bettercloud/refs/heads/main/json-schema/bettercloud-group-schema.json\",\n  \"title\": \"Group\",\n  \"description\": \"A group from an integrated directory service.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the group.\",\n      \"example\": \"group-x1y2z3\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the group.\",\n      \"example\": \"Engineering Team\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"nullable\": true,\n      \"description\": \"Email address of the group.\",\n      \"example\": \"engineering@example.com\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"Description of the\
  \ group.\",\n      \"example\": \"Engineering department group\"\n    },\n    \"member_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of members in the group.\",\n      \"example\": 45\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the group was created.\",\n      \"example\": \"2024-06-01T00:00:00Z\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"nullable\": true,\n      \"description\": \"When the group was last updated.\",\n      \"example\": \"2026-03-01T00:00:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bettercloud/refs/heads/main/json-schema/bettercloud-group-schema.json
tags:
- Automation
- Compliance
- Enterprise
- IT Operations
- SaaS Management
- Security
- Workflows
- User Lifecycle
title: Group
---
