---
description: Call schema from Bandwidth voice API
layout: schema
name: Call
properties_list:
- description: The unique identifier for the call
  name: callId
  type: string
- description: The Bandwidth account ID
  name: accountId
  type: string
- description: The application ID associated with the call
  name: applicationId
  type: string
- description: The destination phone number
  name: to
  type: string
- description: The originating phone number
  name: from
  type: string
- description: The direction of the call
  name: direction
  type: string
- description: The current state of the call
  name: state
  type: string
- description: The time the call was initiated
  name: startTime
  type: string
- description: The time the call was answered
  name: answerTime
  type: string
- description: The time the call ended
  name: endTime
  type: string
- description: The reason the call was disconnected
  name: disconnectCause
  type: string
- description: Custom tag attached to the call
  name: tag
  type: string
- description: The URL for this call resource
  name: callUrl
  type: string
provider_name: Bandwidth
provider_slug: bandwidth
schema_file: json-schema/voice-call-schema.json
slug: voice-call
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
title: Call
---
