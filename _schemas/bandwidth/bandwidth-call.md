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
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.com/schemas/bandwidth/call.json\",\n  \"title\": \"Bandwidth Call\",\n  \"description\": \"Represents a voice call managed through the Bandwidth Voice API, including outbound and inbound calls with state tracking, recording references, and call control metadata.\",\n  \"type\": \"object\",\n  \"required\": [\"from\", \"to\", \"applicationId\"],\n  \"properties\": {\n    \"callId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the call, assigned by Bandwidth\"\n    },\n    \"accountId\": {\n      \"type\": \"string\",\n      \"description\": \"The Bandwidth account ID that owns the call\"\n    },\n    \"applicationId\": {\n      \"type\": \"string\",\n      \"description\": \"The Bandwidth application ID associated with the call\"\n    },\n    \"from\": {\n      \"type\": \"string\",\n      \"pattern\": \"^\\\\+1[2-9]\\\\d{9}$\",\n  \
  \    \"description\": \"The originating phone number in E.164 format\"\n    },\n    \"to\": {\n      \"type\": \"string\",\n      \"pattern\": \"^\\\\+1[2-9]\\\\d{9}$\",\n      \"description\": \"The destination phone number in E.164 format\"\n    },\n    \"direction\": {\n      \"type\": \"string\",\n      \"enum\": [\"inbound\", \"outbound\"],\n      \"description\": \"The direction of the call\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"enum\": [\"initiated\", \"answered\", \"completed\"],\n      \"description\": \"The current state of the call\"\n    },\n    \"answerUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL that receives the answer webhook and returns BXML\"\n    },\n    \"answerMethod\": {\n      \"type\": \"string\",\n      \"enum\": [\"POST\", \"GET\"],\n      \"default\": \"POST\",\n      \"description\": \"The HTTP method for the answer webhook\"\n    },\n    \"disconnectUrl\": {\n      \"type\": \"\
  string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL that receives the disconnect webhook\"\n    },\n    \"disconnectMethod\": {\n      \"type\": \"string\",\n      \"enum\": [\"POST\", \"GET\"],\n      \"default\": \"POST\",\n      \"description\": \"The HTTP method for the disconnect webhook\"\n    },\n    \"startTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The ISO 8601 timestamp when the call was initiated\"\n    },\n    \"answerTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The ISO 8601 timestamp when the call was answered\"\n    },\n    \"endTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The ISO 8601 timestamp when the call ended\"\n    },\n    \"disconnectCause\": {\n      \"type\": \"string\",\n      \"description\": \"The reason the call was disconnected (e.g., hangup, timeout, cancel)\"\n    },\n    \"\
  callTimeout\": {\n      \"type\": \"number\",\n      \"minimum\": 1,\n      \"maximum\": 300,\n      \"default\": 30,\n      \"description\": \"The timeout in seconds for the outbound call to be answered\"\n    },\n    \"callbackTimeout\": {\n      \"type\": \"number\",\n      \"minimum\": 1,\n      \"maximum\": 25,\n      \"default\": 15,\n      \"description\": \"The timeout in seconds for webhook callback requests\"\n    },\n    \"tag\": {\n      \"type\": \"string\",\n      \"maxLength\": 256,\n      \"description\": \"A custom string attached to the call for tracking purposes\"\n    },\n    \"callUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL for this call resource in the Bandwidth API\"\n    }\n  },\n  \"$defs\": {\n    \"Recording\": {\n      \"type\": \"object\",\n      \"description\": \"A recording of a voice call\",\n      \"properties\": {\n        \"recordingId\": {\n          \"type\": \"string\",\n          \"description\"\
  : \"The unique identifier for the recording\"\n        },\n        \"callId\": {\n          \"type\": \"string\",\n          \"description\": \"The call ID associated with this recording\"\n        },\n        \"duration\": {\n          \"type\": \"string\",\n          \"description\": \"The duration of the recording in ISO 8601 format\"\n        },\n        \"channels\": {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"maximum\": 2,\n          \"description\": \"The number of audio channels\"\n        },\n        \"startTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"When the recording started\"\n        },\n        \"endTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"When the recording ended\"\n        },\n        \"fileFormat\": {\n          \"type\": \"string\",\n          \"enum\": [\"wav\", \"mp3\"],\n          \"description\": \"\
  The audio file format\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"enum\": [\"complete\", \"partial\", \"error\"],\n          \"description\": \"The recording status\"\n        },\n        \"mediaUrl\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"The URL to download the recording audio\"\n        }\n      }\n    },\n    \"Conference\": {\n      \"type\": \"object\",\n      \"description\": \"A multi-party conference call\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The unique conference identifier\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The user-defined conference name\"\n        },\n        \"createdTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"When the conference was created\"\n        },\n        \"completedTime\"\
  : {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"When the conference ended\"\n        },\n        \"tag\": {\n          \"type\": \"string\",\n          \"description\": \"Custom tag for the conference\"\n        },\n        \"activeMembers\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/$defs/ConferenceMember\"\n          },\n          \"description\": \"List of active conference members\"\n        }\n      }\n    },\n    \"ConferenceMember\": {\n      \"type\": \"object\",\n      \"description\": \"A member of a conference call\",\n      \"properties\": {\n        \"callId\": {\n          \"type\": \"string\",\n          \"description\": \"The call ID of the conference member\"\n        },\n        \"conferenceId\": {\n          \"type\": \"string\",\n          \"description\": \"The conference ID\"\n        },\n        \"mute\": {\n          \"type\": \"boolean\",\n          \"description\"\
  : \"Whether the member is muted\"\n        },\n        \"hold\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the member is on hold\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/bandwidth-call-schema.json
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
