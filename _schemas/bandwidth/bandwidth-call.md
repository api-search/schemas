---
description: Represents a voice call managed through the Bandwidth Voice API, including outbound and inbound calls with state tracking, recording references, and call control metadata.
layout: schema
name: Bandwidth Call
properties_list:
- description: The unique identifier for the call, assigned by Bandwidth
  name: callId
  type: string
- description: The Bandwidth account ID that owns the call
  name: accountId
  type: string
- description: The Bandwidth application ID associated with the call
  name: applicationId
  type: string
- description: The originating phone number in E.164 format
  name: from
  type: string
- description: The destination phone number in E.164 format
  name: to
  type: string
- description: The direction of the call
  name: direction
  type: string
- description: The current state of the call
  name: state
  type: string
- description: The URL that receives the answer webhook and returns BXML
  name: answerUrl
  type: string
- description: The HTTP method for the answer webhook
  name: answerMethod
  type: string
- description: The URL that receives the disconnect webhook
  name: disconnectUrl
  type: string
- description: The HTTP method for the disconnect webhook
  name: disconnectMethod
  type: string
- description: The ISO 8601 timestamp when the call was initiated
  name: startTime
  type: string
- description: The ISO 8601 timestamp when the call was answered
  name: answerTime
  type: string
- description: The ISO 8601 timestamp when the call ended
  name: endTime
  type: string
- description: The reason the call was disconnected (e.g., hangup, timeout, cancel)
  name: disconnectCause
  type: string
- description: The timeout in seconds for the outbound call to be answered
  name: callTimeout
  type: number
- description: The timeout in seconds for webhook callback requests
  name: callbackTimeout
  type: number
- description: A custom string attached to the call for tracking purposes
  name: tag
  type: string
- description: The URL for this call resource in the Bandwidth API
  name: callUrl
  type: string
provider_name: Bandwidth
provider_slug: bandwidth
schema_file: json-schema/bandwidth-call-schema.json
slug: bandwidth-call
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
title: Bandwidth Call
---
