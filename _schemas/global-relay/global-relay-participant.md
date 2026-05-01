---
description: A participant in a conversation, email, voice call, or event within the Global Relay Archive.
layout: schema
name: Global Relay Participant
properties_list:
- description: Unique identifier for the participant
  name: participantId
  type: string
- description: Display name of the participant
  name: displayName
  type: string
- description: Email address of the participant
  name: email
  type: string
- description: Role of the participant
  name: role
  type: string
provider_name: Global Relay
provider_slug: global-relay
schema_file: json-schema/global-relay-participant.json
slug: global-relay-participant
source_filename: global-relay-participant.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"global-relay-participant.json\",\n  \"title\": \"Global Relay Participant\",\n  \"description\": \"A participant in a conversation, email, voice call, or event within the Global Relay Archive.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"participantId\",\n    \"displayName\"\n  ],\n  \"properties\": {\n    \"participantId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the participant\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the participant\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Email address of the participant\"\n    },\n    \"role\": {\n      \"type\": \"string\",\n      \"description\": \"Role of the participant\",\n      \"enum\": [\n        \"Host\",\n        \"Presenter\",\n        \"Attendee\",\n        \"Caller\"\
  ,\n        \"Callee\",\n        \"Sender\",\n        \"Recipient\"\n      ]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/global-relay/refs/heads/main/json-schema/global-relay-participant.json
tags:
- Archiving
- Compliance
- Data Retention
- Email Security
- Regulatory Compliance
title: Global Relay Participant
---
