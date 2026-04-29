---
description: Represents a channel in a team.
layout: schema
name: Channel
properties_list:
- description: Unique identifier for the channel.
  name: id
  type: string
- description: The display name of the channel.
  name: displayName
  type: string
- description: Description of the channel.
  name: description
  type: string
- description: Type of membership for the channel.
  name: membershipType
  type: string
- description: When the channel was created.
  name: createdDateTime
  type: string
- description: URL to the channel in Teams.
  name: webUrl
  type: string
provider_name: Microsoft Teams
provider_slug: microsoft-teams
schema_file: json-schema/teams-graph-api-channel-schema.json
slug: teams-graph-api-channel
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/microsoft-teams/refs/heads/main/json-schema/teams-graph-api-channel-schema.json\",\n  \"title\": \"Channel\",\n  \"description\": \"Represents a channel in a team.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": { \"type\": \"string\", \"description\": \"Unique identifier for the channel.\" },\n    \"displayName\": { \"type\": \"string\", \"description\": \"The display name of the channel.\" },\n    \"description\": { \"type\": \"string\", \"description\": \"Description of the channel.\" },\n    \"membershipType\": { \"type\": \"string\", \"enum\": [\"standard\", \"private\", \"shared\"], \"description\": \"Type of membership for the channel.\" },\n    \"createdDateTime\": { \"type\": \"string\", \"format\": \"date-time\", \"description\": \"When the channel was created.\" },\n    \"webUrl\": { \"type\": \"string\", \"format\": \"\
  uri\", \"description\": \"URL to the channel in Teams.\" }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-teams/refs/heads/main/json-schema/teams-graph-api-channel-schema.json
tags:
- Chat
- Collaboration
- Communication
- Microsoft 365
- Productivity
- Video Conferencing
title: Channel
---
