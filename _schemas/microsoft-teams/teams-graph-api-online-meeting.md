---
description: Represents an online meeting in Teams.
layout: schema
name: OnlineMeeting
properties_list:
- description: Unique identifier for the meeting.
  name: id
  type: string
- description: Subject of the meeting.
  name: subject
  type: string
- description: Start time of the meeting.
  name: startDateTime
  type: string
- description: End time of the meeting.
  name: endDateTime
  type: string
- description: URL to join the meeting.
  name: joinWebUrl
  type: string
provider_name: Microsoft Teams
provider_slug: microsoft-teams
schema_file: json-schema/teams-graph-api-online-meeting-schema.json
slug: teams-graph-api-online-meeting
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/microsoft-teams/refs/heads/main/json-schema/teams-graph-api-online-meeting-schema.json\",\n  \"title\": \"OnlineMeeting\",\n  \"description\": \"Represents an online meeting in Teams.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": { \"type\": \"string\", \"description\": \"Unique identifier for the meeting.\" },\n    \"subject\": { \"type\": \"string\", \"description\": \"Subject of the meeting.\" },\n    \"startDateTime\": { \"type\": \"string\", \"format\": \"date-time\", \"description\": \"Start time of the meeting.\" },\n    \"endDateTime\": { \"type\": \"string\", \"format\": \"date-time\", \"description\": \"End time of the meeting.\" },\n    \"joinWebUrl\": { \"type\": \"string\", \"format\": \"uri\", \"description\": \"URL to join the meeting.\" }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-teams/refs/heads/main/json-schema/teams-graph-api-online-meeting-schema.json
tags:
- Chat
- Collaboration
- Communication
- Microsoft 365
- Productivity
- Video Conferencing
title: OnlineMeeting
---
