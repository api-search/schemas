---
description: A paginated list of user resources.
layout: schema
name: Users
properties_list:
- description: The type of the API resource.
  name: kind
  type: string
- description: ETag of the resource.
  name: etag
  type: string
- description: A list of user objects.
  name: users
  type: array
- description: Token for retrieving the next page of results.
  name: nextPageToken
  type: string
- description: Event that triggered this response (for push notifications).
  name: trigger_event
  type: string
provider_name: Google Workspace
provider_slug: google-workspace
schema_file: json-schema/admin-sdk-directory-users-schema.json
slug: admin-sdk-directory-users
source_filename: admin-sdk-directory-users-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Users\",\n  \"type\": \"object\",\n  \"description\": \"A paginated list of user resources.\",\n  \"properties\": {\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the API resource.\"\n    },\n    \"etag\": {\n      \"type\": \"string\",\n      \"description\": \"ETag of the resource.\"\n    },\n    \"users\": {\n      \"type\": \"array\",\n      \"description\": \"A list of user objects.\"\n    },\n    \"nextPageToken\": {\n      \"type\": \"string\",\n      \"description\": \"Token for retrieving the next page of results.\"\n    },\n    \"trigger_event\": {\n      \"type\": \"string\",\n      \"description\": \"Event that triggered this response (for push notifications).\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-workspace/refs/heads/main/json-schema/admin-sdk-directory-users-schema.json
tags:
- Calendar
- Collaboration
- Email
- Productivity
- Storage
- Video Conferencing
title: Users
---
