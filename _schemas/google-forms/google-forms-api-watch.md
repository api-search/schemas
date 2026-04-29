---
description: A watch for receiving notifications about form changes or responses.
layout: schema
name: Watch
properties_list:
- description: Output only. The ID of this watch.
  name: id
  type: string
- description: The target for watch notifications.
  name: target
  type: object
- description: Which event type to watch for.
  name: eventType
  type: string
- description: Timestamp of when this was created.
  name: createTime
  type: string
- description: Timestamp for when this will expire.
  name: expireTime
  type: string
- description: ''
  name: errorType
  type: string
- description: ''
  name: state
  type: string
provider_name: Google Forms
provider_slug: google-forms
schema_file: json-schema/google-forms-api-watch-schema.json
slug: google-forms-api-watch
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/google-forms/refs/heads/main/json-schema/google-forms-api-watch-schema.json\",\n  \"title\": \"Watch\",\n  \"description\": \"A watch for receiving notifications about form changes or responses.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": { \"type\": \"string\", \"description\": \"Output only. The ID of this watch.\", \"readOnly\": true },\n    \"target\": {\n      \"type\": \"object\",\n      \"description\": \"The target for watch notifications.\",\n      \"properties\": {\n        \"topic\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"topicName\": { \"type\": \"string\", \"description\": \"A fully qualified Pub/Sub topic name.\" }\n          }\n        }\n      }\n    },\n    \"eventType\": {\n      \"type\": \"string\",\n      \"description\": \"Which event type to watch for.\",\n      \"\
  enum\": [\"EVENT_TYPE_UNSPECIFIED\", \"SCHEMA\", \"RESPONSES\"]\n    },\n    \"createTime\": { \"type\": \"string\", \"format\": \"date-time\", \"description\": \"Timestamp of when this was created.\" },\n    \"expireTime\": { \"type\": \"string\", \"format\": \"date-time\", \"description\": \"Timestamp for when this will expire.\" },\n    \"errorType\": {\n      \"type\": \"string\",\n      \"enum\": [\"ERROR_TYPE_UNSPECIFIED\", \"PROJECT_NOT_AUTHORIZED\", \"NO_USER_ACCESS\", \"OTHER_ERRORS\"]\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"enum\": [\"STATE_UNSPECIFIED\", \"ACTIVE\", \"SUSPENDED\"]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-forms/refs/heads/main/json-schema/google-forms-api-watch-schema.json
tags:
- Data Collection
- Forms
- Google
- Google Workspace
- Questionnaires
- Responses
- Surveys
title: Watch
---
