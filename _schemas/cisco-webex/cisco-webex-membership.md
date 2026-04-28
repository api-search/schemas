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
tags:
- Collaboration
- Communications
- Meetings
- Messaging
- Teams
- Video Conferencing
title: Cisco Webex Membership
---
