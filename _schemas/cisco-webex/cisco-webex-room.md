---
description: Represents a Webex room (space) where people post messages and collaborate. Rooms can be direct (1:1) or group conversations, and can be organized within teams.
layout: schema
name: Cisco Webex Room
properties_list:
- description: Unique identifier for the room.
  name: id
  type: string
- description: A user-friendly name for the room.
  name: title
  type: string
- description: The type of room.
  name: type
  type: string
- description: Whether the room is moderated.
  name: isLocked
  type: boolean
- description: Whether the room is public and discoverable within the organization.
  name: isPublic
  type: boolean
- description: Whether only moderators can post messages.
  name: isAnnouncementOnly
  type: boolean
- description: Whether the room is read-only.
  name: isReadOnly
  type: boolean
- description: The team ID associated with the room.
  name: teamId
  type: string
- description: Date and time of the last activity in the room.
  name: lastActivity
  type: string
- description: The person ID of the room creator.
  name: creatorId
  type: string
- description: The person ID of the room owner.
  name: ownerId
  type: string
- description: The classification ID of the room.
  name: classificationId
  type: string
- description: The description of the room.
  name: description
  type: string
- description: Date and time the room was made public.
  name: madePublic
  type: string
- description: Date and time the room was created.
  name: created
  type: string
provider_name: Cisco Webex
provider_slug: cisco-webex
schema_file: json-schema/cisco-webex-room-schema.json
slug: cisco-webex-room
source_filename: cisco-webex-room-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.webex.com/schemas/room.json\",\n  \"title\": \"Cisco Webex Room\",\n  \"description\": \"Represents a Webex room (space) where people post messages and collaborate. Rooms can be direct (1:1) or group conversations, and can be organized within teams.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the room.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"A user-friendly name for the room.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of room.\",\n      \"enum\": [\"direct\", \"group\"]\n    },\n    \"isLocked\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the room is moderated.\"\n    },\n    \"isPublic\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the room is public\
  \ and discoverable within the organization.\"\n    },\n    \"isAnnouncementOnly\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether only moderators can post messages.\"\n    },\n    \"isReadOnly\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the room is read-only.\"\n    },\n    \"teamId\": {\n      \"type\": \"string\",\n      \"description\": \"The team ID associated with the room.\"\n    },\n    \"lastActivity\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time of the last activity in the room.\"\n    },\n    \"creatorId\": {\n      \"type\": \"string\",\n      \"description\": \"The person ID of the room creator.\"\n    },\n    \"ownerId\": {\n      \"type\": \"string\",\n      \"description\": \"The person ID of the room owner.\"\n    },\n    \"classificationId\": {\n      \"type\": \"string\",\n      \"description\": \"The classification ID of the room.\"\n    },\n    \"description\": {\n\
  \      \"type\": \"string\",\n      \"description\": \"The description of the room.\"\n    },\n    \"madePublic\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time the room was made public.\"\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time the room was created.\"\n    }\n  },\n  \"required\": [\"id\", \"title\", \"type\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cisco-webex/refs/heads/main/json-schema/cisco-webex-room-schema.json
tags:
- Collaboration
- Communications
- Meetings
- Messaging
- Teams
- Video Conferencing
title: Cisco Webex Room
---
