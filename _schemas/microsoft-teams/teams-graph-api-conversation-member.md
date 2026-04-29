---
description: Represents a member of a team or channel.
layout: schema
name: ConversationMember
properties_list:
- description: Unique membership ID.
  name: id
  type: string
- description: Display name of the member.
  name: displayName
  type: string
- description: Roles of the member.
  name: roles
  type: array
- description: The Azure AD user ID.
  name: userId
  type: string
- description: Email address of the member.
  name: email
  type: string
provider_name: Microsoft Teams
provider_slug: microsoft-teams
schema_file: json-schema/teams-graph-api-conversation-member-schema.json
slug: teams-graph-api-conversation-member
source_filename: teams-graph-api-conversation-member-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/microsoft-teams/refs/heads/main/json-schema/teams-graph-api-conversation-member-schema.json\",\n  \"title\": \"ConversationMember\",\n  \"description\": \"Represents a member of a team or channel.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": { \"type\": \"string\", \"description\": \"Unique membership ID.\" },\n    \"displayName\": { \"type\": \"string\", \"description\": \"Display name of the member.\" },\n    \"roles\": { \"type\": \"array\", \"items\": { \"type\": \"string\" }, \"description\": \"Roles of the member.\" },\n    \"userId\": { \"type\": \"string\", \"description\": \"The Azure AD user ID.\" },\n    \"email\": { \"type\": \"string\", \"format\": \"email\", \"description\": \"Email address of the member.\" }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-teams/refs/heads/main/json-schema/teams-graph-api-conversation-member-schema.json
tags:
- Chat
- Collaboration
- Communication
- Microsoft 365
- Productivity
- Video Conferencing
title: ConversationMember
---
