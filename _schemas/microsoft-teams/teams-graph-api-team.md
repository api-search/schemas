---
description: Represents a Microsoft Teams team.
layout: schema
name: Team
properties_list:
- description: Unique identifier for the team.
  name: id
  type: string
- description: The display name of the team.
  name: displayName
  type: string
- description: Description of the team.
  name: description
  type: string
- description: Team visibility.
  name: visibility
  type: string
- description: Whether the team is archived.
  name: isArchived
  type: boolean
- description: When the team was created.
  name: createdDateTime
  type: string
- description: URL to the team in Microsoft Teams.
  name: webUrl
  type: string
provider_name: Microsoft Teams
provider_slug: microsoft-teams
schema_file: json-schema/teams-graph-api-team-schema.json
slug: teams-graph-api-team
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/microsoft-teams/refs/heads/main/json-schema/teams-graph-api-team-schema.json\",\n  \"title\": \"Team\",\n  \"description\": \"Represents a Microsoft Teams team.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": { \"type\": \"string\", \"description\": \"Unique identifier for the team.\" },\n    \"displayName\": { \"type\": \"string\", \"description\": \"The display name of the team.\" },\n    \"description\": { \"type\": \"string\", \"description\": \"Description of the team.\" },\n    \"visibility\": { \"type\": \"string\", \"enum\": [\"public\", \"private\"], \"description\": \"Team visibility.\" },\n    \"isArchived\": { \"type\": \"boolean\", \"description\": \"Whether the team is archived.\" },\n    \"createdDateTime\": { \"type\": \"string\", \"format\": \"date-time\", \"description\": \"When the team was created.\" },\n    \"\
  webUrl\": { \"type\": \"string\", \"format\": \"uri\", \"description\": \"URL to the team in Microsoft Teams.\" }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-teams/refs/heads/main/json-schema/teams-graph-api-team-schema.json
tags:
- Chat
- Collaboration
- Communication
- Microsoft 365
- Productivity
- Video Conferencing
title: Team
---
