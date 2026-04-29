---
description: MfaVerifyRequest schema from Bandwidth mfa API
layout: schema
name: MfaVerifyRequest
properties_list:
- description: The phone number the MFA code was sent to, in E.164 format
  name: to
  type: string
- description: The scope that was used when the code was generated. Must match for verification to succeed.
  name: scope
  type: string
- description: The MFA code entered by the user for verification
  name: code
  type: string
- description: The expiration window to check against, in minutes
  name: expirationTimeInMinutes
  type: number
provider_name: Bandwidth
provider_slug: bandwidth
schema_file: json-schema/mfa-mfa-verify-request-schema.json
slug: mfa-mfa-verify-request
source_filename: mfa-mfa-verify-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/mfa-mfa-verify-request-schema.json\",\n  \"title\": \"MfaVerifyRequest\",\n  \"description\": \"MfaVerifyRequest schema from Bandwidth mfa API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"to\": {\n      \"type\": \"string\",\n      \"description\": \"The phone number the MFA code was sent to, in E.164 format\",\n      \"example\": \"+19195554321\"\n    },\n    \"scope\": {\n      \"type\": \"string\",\n      \"description\": \"The scope that was used when the code was generated. Must match for verification to succeed.\"\n    },\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"The MFA code entered by the user for verification\",\n      \"example\": \"123456\"\n    },\n    \"expirationTimeInMinutes\": {\n      \"type\": \"number\",\n      \"minimum\": 1,\n      \"maximum\": 15,\n\
  \      \"default\": 3,\n      \"description\": \"The expiration window to check against, in minutes\"\n    }\n  },\n  \"required\": [\n    \"to\",\n    \"code\",\n    \"expirationTimeInMinutes\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/mfa-mfa-verify-request-schema.json
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
title: MfaVerifyRequest
---
