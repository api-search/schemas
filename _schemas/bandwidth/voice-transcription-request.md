---
description: TranscriptionRequest schema from Bandwidth voice API
layout: schema
name: TranscriptionRequest
properties_list:
- description: The URL to send the transcription completed webhook to
  name: callbackUrl
  type: string
- description: The HTTP method for the transcription webhook
  name: callbackMethod
  type: string
- description: Custom tag for the transcription request
  name: tag
  type: string
provider_name: Bandwidth
provider_slug: bandwidth
schema_file: json-schema/voice-transcription-request-schema.json
slug: voice-transcription-request
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
title: TranscriptionRequest
---
