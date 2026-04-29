---
description: MfaVoiceResponse schema from Bandwidth mfa API
layout: schema
name: MfaVoiceResponse
properties_list:
- description: The unique identifier for the voice call made with the MFA code
  name: callId
  type: string
provider_name: Bandwidth
provider_slug: bandwidth
schema_file: json-schema/mfa-mfa-voice-response-schema.json
slug: mfa-mfa-voice-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/mfa-mfa-voice-response-schema.json\",\n  \"title\": \"MfaVoiceResponse\",\n  \"description\": \"MfaVoiceResponse schema from Bandwidth mfa API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"callId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the voice call made with the MFA code\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/mfa-mfa-voice-response-schema.json
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
title: MfaVoiceResponse
---
