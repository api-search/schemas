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
tags:
- Collaboration
- Communications
- Meetings
- Messaging
- Teams
- Video Conferencing
title: Cisco Webex Room
---
