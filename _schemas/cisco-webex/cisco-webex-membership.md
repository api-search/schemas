---
description: Represents a person's relationship to a Webex room, including their role and access permissions.
layout: schema
name: Cisco Webex Membership
properties_list:
- description: Unique identifier for the membership.
  name: id
  type: string
- description: The room ID for the membership.
  name: roomId
  type: string
- description: The person ID for the membership.
  name: personId
  type: string
- description: The email address of the person.
  name: personEmail
  type: string
- description: The display name of the person.
  name: personDisplayName
  type: string
- description: The organization ID of the person.
  name: personOrgId
  type: string
- description: Whether the person is a room moderator.
  name: isModerator
  type: boolean
- description: Whether the direct space is hidden for this member.
  name: isRoomHidden
  type: boolean
- description: The type of room.
  name: roomType
  type: string
- description: Whether the member is a monitoring bot.
  name: isMonitor
  type: boolean
- description: Date and time the membership was created.
  name: created
  type: string
provider_name: Cisco Webex
provider_slug: cisco-webex
schema_file: json-schema/cisco-webex-membership-schema.json
slug: cisco-webex-membership
source_filename: cisco-webex-membership-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.webex.com/schemas/membership.json\",\n  \"title\": \"Cisco Webex Membership\",\n  \"description\": \"Represents a person's relationship to a Webex room, including their role and access permissions.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the membership.\"\n    },\n    \"roomId\": {\n      \"type\": \"string\",\n      \"description\": \"The room ID for the membership.\"\n    },\n    \"personId\": {\n      \"type\": \"string\",\n      \"description\": \"The person ID for the membership.\"\n    },\n    \"personEmail\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"The email address of the person.\"\n    },\n    \"personDisplayName\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the person.\"\n    },\n    \"\
  personOrgId\": {\n      \"type\": \"string\",\n      \"description\": \"The organization ID of the person.\"\n    },\n    \"isModerator\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the person is a room moderator.\"\n    },\n    \"isRoomHidden\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the direct space is hidden for this member.\"\n    },\n    \"roomType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of room.\",\n      \"enum\": [\"direct\", \"group\"]\n    },\n    \"isMonitor\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the member is a monitoring bot.\"\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time the membership was created.\"\n    }\n  },\n  \"required\": [\"id\", \"roomId\", \"personId\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cisco-webex/refs/heads/main/json-schema/cisco-webex-membership-schema.json
tags:
- Collaboration
- Communications
- Meetings
- Messaging
- Teams
- Video Conferencing
title: Cisco Webex Membership
---
