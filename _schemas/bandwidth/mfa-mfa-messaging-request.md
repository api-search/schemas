---
description: MfaMessagingRequest schema from Bandwidth mfa API
layout: schema
name: MfaMessagingRequest
properties_list:
- description: The Bandwidth phone number to send the SMS from, in E.164 format
  name: from
  type: string
- description: The destination phone number to send the MFA code to, in E.164 format
  name: to
  type: string
- description: The ID of the Bandwidth messaging application to use for sending the SMS
  name: applicationId
  type: string
- description: An optional field to denote what scope or action the MFA code is for. This is returned during verification.
  name: scope
  type: string
- description: The message template to send. Use {CODE} as a placeholder for the generated MFA code.
  name: message
  type: string
- description: The number of digits in the generated MFA code (4-8)
  name: digits
  type: integer
- description: The time in minutes before the MFA code expires (1-15, default 3 minutes)
  name: expirationTimeInMinutes
  type: number
provider_name: Bandwidth
provider_slug: bandwidth
schema_file: json-schema/mfa-mfa-messaging-request-schema.json
slug: mfa-mfa-messaging-request
source_filename: mfa-mfa-messaging-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/mfa-mfa-messaging-request-schema.json\",\n  \"title\": \"MfaMessagingRequest\",\n  \"description\": \"MfaMessagingRequest schema from Bandwidth mfa API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"from\": {\n      \"type\": \"string\",\n      \"description\": \"The Bandwidth phone number to send the SMS from, in E.164 format\",\n      \"example\": \"+19195551234\"\n    },\n    \"to\": {\n      \"type\": \"string\",\n      \"description\": \"The destination phone number to send the MFA code to, in E.164 format\",\n      \"example\": \"+19195554321\"\n    },\n    \"applicationId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the Bandwidth messaging application to use for sending the SMS\"\n    },\n    \"scope\": {\n      \"type\": \"string\",\n      \"description\": \"An optional\
  \ field to denote what scope or action the MFA code is for. This is returned during verification.\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"The message template to send. Use {CODE} as a placeholder for the generated MFA code.\",\n      \"example\": \"Your verification code is {CODE}\"\n    },\n    \"digits\": {\n      \"type\": \"integer\",\n      \"minimum\": 4,\n      \"maximum\": 8,\n      \"description\": \"The number of digits in the generated MFA code (4-8)\",\n      \"example\": 6\n    },\n    \"expirationTimeInMinutes\": {\n      \"type\": \"number\",\n      \"minimum\": 1,\n      \"maximum\": 15,\n      \"default\": 3,\n      \"description\": \"The time in minutes before the MFA code expires (1-15, default 3 minutes)\"\n    }\n  },\n  \"required\": [\n    \"from\",\n    \"to\",\n    \"applicationId\",\n    \"message\",\n    \"digits\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/mfa-mfa-messaging-request-schema.json
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
title: MfaMessagingRequest
---
