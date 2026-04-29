---
description: The request body for fetching events. Must include either a cursor string from a previous response to continue pagination, or a ResetCursor object to start fetching from a specific time.
layout: schema
name: EventRequest
properties_list:
- description: The maximum number of event records to return per page.
  name: limit
  type: integer
- description: A cursor from a previous response to continue fetching events from where the last request left off.
  name: cursor
  type: string
- description: An ISO 8601 timestamp to begin fetching events from a specific time. Used to create a new cursor starting from this point.
  name: start_time
  type: string
provider_name: 1Password
provider_slug: 1password
schema_file: json-schema/1password-events-event-request-schema.json
slug: 1password-events-event-request
source_filename: 1password-events-event-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/json-schema/1password-events-event-request-schema.json\",\n  \"title\": \"EventRequest\",\n  \"description\": \"The request body for fetching events. Must include either a cursor string from a previous response to continue pagination, or a ResetCursor object to start fetching from a specific time.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"limit\": {\n      \"type\": \"integer\",\n      \"description\": \"The maximum number of event records to return per page.\",\n      \"minimum\": 1,\n      \"maximum\": 1000,\n      \"default\": 100\n    },\n    \"cursor\": {\n      \"type\": \"string\",\n      \"description\": \"A cursor from a previous response to continue fetching events from where the last request left off.\"\n    },\n    \"start_time\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\
  ,\n      \"description\": \"An ISO 8601 timestamp to begin fetching events from a specific time. Used to create a new cursor starting from this point.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/json-schema/1password-events-event-request-schema.json
tags:
- Password Manager
- Passwords
- Security
- Secrets
title: EventRequest
---
