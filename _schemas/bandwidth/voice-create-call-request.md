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
source_filename: voice-create-call-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/voice-create-call-request-schema.json\",\n  \"title\": \"CreateCallRequest\",\n  \"description\": \"CreateCallRequest schema from Bandwidth voice API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"from\": {\n      \"type\": \"string\",\n      \"description\": \"The Bandwidth phone number that will make the outbound call, in E.164 format\",\n      \"example\": \"+19195551234\"\n    },\n    \"to\": {\n      \"type\": \"string\",\n      \"description\": \"The destination phone number for the outbound call, in E.164 format\",\n      \"example\": \"+19195554321\"\n    },\n    \"answerUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL to send the answer webhook to when the call is answered. The endpoint should return BXML to control the call flow.\"\n    },\n\
  \    \"answerMethod\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"POST\",\n        \"GET\"\n      ],\n      \"default\": \"POST\",\n      \"description\": \"The HTTP method to use for the answer webhook\"\n    },\n    \"answerFallbackUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Fallback URL for the answer webhook if the primary URL fails\"\n    },\n    \"answerFallbackMethod\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"POST\",\n        \"GET\"\n      ],\n      \"default\": \"POST\",\n      \"description\": \"The HTTP method for the fallback answer webhook\"\n    },\n    \"disconnectUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL to send the disconnect webhook to when the call ends\"\n    },\n    \"disconnectMethod\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"POST\",\n        \"GET\"\n      ],\n      \"default\": \"POST\",\n      \"description\"\
  : \"The HTTP method for the disconnect webhook\"\n    },\n    \"applicationId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the Bandwidth application associated with this call\"\n    },\n    \"tag\": {\n      \"type\": \"string\",\n      \"maxLength\": 256,\n      \"description\": \"A custom string to attach to the call for tracking purposes\"\n    },\n    \"callTimeout\": {\n      \"type\": \"number\",\n      \"minimum\": 1,\n      \"maximum\": 300,\n      \"default\": 30,\n      \"description\": \"The timeout in seconds for the outbound call to be answered\"\n    },\n    \"callbackTimeout\": {\n      \"type\": \"number\",\n      \"minimum\": 1,\n      \"maximum\": 25,\n      \"default\": 15,\n      \"description\": \"The timeout in seconds for webhook callback requests\"\n    }\n  },\n  \"required\": [\n    \"from\",\n    \"to\",\n    \"answerUrl\",\n    \"applicationId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/voice-create-call-request-schema.json
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
