---
description: Recording schema from Bandwidth voice API
layout: schema
name: Recording
properties_list:
- description: The unique identifier for the recording
  name: recordingId
  type: string
- description: The Bandwidth account ID
  name: accountId
  type: string
- description: The call ID associated with this recording
  name: callId
  type: string
- description: The application ID
  name: applicationId
  type: string
- description: The duration of the recording in ISO 8601 format
  name: duration
  type: string
- description: The number of audio channels in the recording
  name: channels
  type: integer
- description: The time the recording started
  name: startTime
  type: string
- description: The time the recording ended
  name: endTime
  type: string
- description: The audio format of the recording
  name: fileFormat
  type: string
- description: The status of the recording
  name: status
  type: string
- description: The URL to download the recording media
  name: mediaUrl
  type: string
- description: ''
  name: transcription
  type: object
provider_name: Bandwidth
provider_slug: bandwidth
schema_file: json-schema/voice-recording-schema.json
slug: voice-recording
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
title: Recording
---
