---
description: Represents an SMS or MMS message sent or received through the Bandwidth Messaging API, including delivery status, media attachments, and routing metadata.
layout: schema
name: Bandwidth Message
properties_list:
- description: The unique identifier for the message, assigned by Bandwidth
  name: id
  type: string
- description: The Bandwidth phone number that owns the message
  name: owner
  type: string
- description: The Bandwidth application ID associated with the message
  name: applicationId
  type: string
- description: The source phone number in E.164 format
  name: from
  type: string
- description: Array of destination phone numbers in E.164 format
  name: to
  type: array
- description: The text content of the message
  name: text
  type: string
- description: Array of media URLs for MMS attachments
  name: media
  type: array
- description: The direction of the message (in for received, out for sent)
  name: direction
  type: string
- description: The number of segments the message was split into for delivery
  name: segmentCount
  type: integer
- description: The ISO 8601 timestamp when the message was created
  name: time
  type: string
- description: A custom string attached to the message for tracking
  name: tag
  type: string
- description: The priority level of the message
  name: priority
  type: string
- description: The expiration time after which undelivered messages are discarded
  name: expiration
  type: string
provider_name: Bandwidth
provider_slug: bandwidth
schema_file: json-schema/bandwidth-message-schema.json
slug: bandwidth-message
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
title: Bandwidth Message
---
