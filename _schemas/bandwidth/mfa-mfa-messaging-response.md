---
description: MfaMessagingResponse schema from Bandwidth mfa API
layout: schema
name: MfaMessagingResponse
properties_list:
- description: The unique identifier for the SMS message sent with the MFA code
  name: messageId
  type: string
provider_name: Bandwidth
provider_slug: bandwidth
schema_file: json-schema/mfa-mfa-messaging-response-schema.json
slug: mfa-mfa-messaging-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/mfa-mfa-messaging-response-schema.json\",\n  \"title\": \"MfaMessagingResponse\",\n  \"description\": \"MfaMessagingResponse schema from Bandwidth mfa API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"messageId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the SMS message sent with the MFA code\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/mfa-mfa-messaging-response-schema.json
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
title: MfaMessagingResponse
---
