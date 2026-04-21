---
description: CreateMessageRequest schema from Bandwidth messaging API
layout: schema
name: CreateMessageRequest
properties_list:
- description: The Bandwidth phone number to send the message from, in E.164 format
  name: from
  type: string
- description: Array of destination phone numbers in E.164 format. Up to 50 numbers for group messaging.
  name: to
  type: array
- description: The text content of the message. Required for SMS. For MMS, text is optional if media is provided.
  name: text
  type: string
- description: Array of media URLs to include as MMS attachments. Each URL must be publicly accessible or a Bandwidth media URL.
  name: media
  type: array
- description: The ID of the Bandwidth application associated with this message. This determines which webhook URLs receive delivery callbacks.
  name: applicationId
  type: string
- description: A custom string to attach to the message for tracking purposes
  name: tag
  type: string
- description: The priority of the message. High priority messages are delivered faster but may incur additional charges.
  name: priority
  type: string
- description: The expiration time for the message. Messages not delivered by this time will be discarded.
  name: expiration
  type: string
provider_name: Bandwidth
provider_slug: bandwidth
schema_file: json-schema/messaging-create-message-request-schema.json
slug: messaging-create-message-request
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
title: CreateMessageRequest
---
