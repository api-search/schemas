---
description: A user discovered and managed across BetterCloud integrations.
layout: schema
name: User
properties_list:
- description: Unique identifier for the user in BetterCloud.
  name: id
  type: string
- description: Primary email address of the user.
  name: email
  type: string
- description: User's first name.
  name: first_name
  type: string
- description: User's last name.
  name: last_name
  type: string
- description: Current status of the user.
  name: status
  type: string
- description: Department or organizational unit.
  name: department
  type: string
- description: Job title.
  name: title
  type: string
- description: Email of the user's manager.
  name: manager_email
  type: string
- description: Office location.
  name: location
  type: string
- description: When the user was first discovered.
  name: created_at
  type: string
- description: When the user record was last updated.
  name: updated_at
  type: string
provider_name: BetterCloud
provider_slug: bettercloud
schema_file: json-schema/bettercloud-user-schema.json
slug: bettercloud-user
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bettercloud/refs/heads/main/json-schema/bettercloud-user-schema.json\",\n  \"title\": \"User\",\n  \"description\": \"A user discovered and managed across BetterCloud integrations.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the user in BetterCloud.\",\n      \"example\": \"user-a1b2c3d4\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Primary email address of the user.\",\n      \"example\": \"jsmith@example.com\"\n    },\n    \"first_name\": {\n      \"type\": \"string\",\n      \"description\": \"User's first name.\",\n      \"example\": \"Jane\"\n    },\n    \"last_name\": {\n      \"type\": \"string\",\n      \"description\": \"User's last name.\",\n      \"example\": \"Smith\"\n  \
  \  },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current status of the user.\",\n      \"enum\": [\n        \"active\",\n        \"suspended\",\n        \"deprovisioned\"\n      ],\n      \"example\": \"active\"\n    },\n    \"department\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"Department or organizational unit.\",\n      \"example\": \"Engineering\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"Job title.\",\n      \"example\": \"Senior Engineer\"\n    },\n    \"manager_email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"nullable\": true,\n      \"description\": \"Email of the user's manager.\",\n      \"example\": \"manager@example.com\"\n    },\n    \"location\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"Office location.\",\n      \"example\": \"San Francisco\"\n    },\n    \"created_at\"\
  : {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the user was first discovered.\",\n      \"example\": \"2025-01-15T10:00:00Z\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the user record was last updated.\",\n      \"example\": \"2026-04-01T08:30:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bettercloud/refs/heads/main/json-schema/bettercloud-user-schema.json
tags:
- Automation
- Compliance
- Enterprise
- IT Operations
- SaaS Management
- Security
- Workflows
- User Lifecycle
title: User
---
