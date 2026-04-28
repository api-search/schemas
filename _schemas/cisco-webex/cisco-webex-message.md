---
description: Represents a message posted in a Webex room, including text, markdown, files, and adaptive card attachments.
layout: schema
name: Cisco Webex Message
properties_list:
- description: Unique identifier for the message.
  name: id
  type: string
- description: The parent message ID if this is a threaded reply.
  name: parentId
  type: string
- description: The room ID where the message was posted.
  name: roomId
  type: string
- description: The type of room.
  name: roomType
  type: string
- description: The plain text content of the message.
  name: text
  type: string
- description: The message content in markdown format.
  name: markdown
  type: string
- description: The rendered HTML content of the message.
  name: html
  type: string
- description: Public URLs for files attached to the message.
  name: files
  type: array
- description: The person ID of the message author.
  name: personId
  type: string
- description: The email address of the message author.
  name: personEmail
  type: string
- description: Person IDs of those mentioned in the message.
  name: mentionedPeople
  type: array
- description: Group names mentioned in the message.
  name: mentionedGroups
  type: array
- description: Adaptive card attachments on the message.
  name: attachments
  type: array
- description: Whether the message is a voice clip.
  name: isVoiceClip
  type: boolean
- description: The date and time the message was created.
  name: created
  type: string
- description: The date and time the message was last updated.
  name: updated
  type: string
provider_name: Cisco Webex
provider_slug: cisco-webex
schema_file: json-schema/cisco-webex-message-schema.json
slug: cisco-webex-message
tags:
- Collaboration
- Communications
- Meetings
- Messaging
- Teams
- Video Conferencing
title: Cisco Webex Message
---
