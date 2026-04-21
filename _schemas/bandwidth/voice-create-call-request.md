---
description: CreateCallRequest schema from Bandwidth voice API
layout: schema
name: CreateCallRequest
properties_list:
- description: The Bandwidth phone number that will make the outbound call, in E.164 format
  name: from
  type: string
- description: The destination phone number for the outbound call, in E.164 format
  name: to
  type: string
- description: The URL to send the answer webhook to when the call is answered. The endpoint should return BXML to control the call flow.
  name: answerUrl
  type: string
- description: The HTTP method to use for the answer webhook
  name: answerMethod
  type: string
- description: Fallback URL for the answer webhook if the primary URL fails
  name: answerFallbackUrl
  type: string
- description: The HTTP method for the fallback answer webhook
  name: answerFallbackMethod
  type: string
- description: The URL to send the disconnect webhook to when the call ends
  name: disconnectUrl
  type: string
- description: The HTTP method for the disconnect webhook
  name: disconnectMethod
  type: string
- description: The ID of the Bandwidth application associated with this call
  name: applicationId
  type: string
- description: A custom string to attach to the call for tracking purposes
  name: tag
  type: string
- description: The timeout in seconds for the outbound call to be answered
  name: callTimeout
  type: number
- description: The timeout in seconds for webhook callback requests
  name: callbackTimeout
  type: number
provider_name: Bandwidth
provider_slug: bandwidth
schema_file: json-schema/voice-create-call-request-schema.json
slug: voice-create-call-request
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
title: CreateCallRequest
---
