---
description: A recipient for emergency call notifications
layout: schema
name: NotificationRecipient
properties_list:
- description: The unique identifier for the notification recipient
  name: id
  type: string
- description: The email address for notifications
  name: emailAddress
  type: string
- description: The phone number for SMS notifications
  name: phoneNumber
  type: string
- description: A description of the notification recipient
  name: description
  type: string
provider_name: Bandwidth
provider_slug: bandwidth
schema_file: json-schema/emergency-calling-notification-recipient-schema.json
slug: emergency-calling-notification-recipient
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/emergency-calling-notification-recipient-schema.json\",\n  \"title\": \"NotificationRecipient\",\n  \"description\": \"A recipient for emergency call notifications\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the notification recipient\"\n    },\n    \"emailAddress\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"The email address for notifications\"\n    },\n    \"phoneNumber\": {\n      \"type\": \"string\",\n      \"description\": \"The phone number for SMS notifications\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the notification recipient\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/emergency-calling-notification-recipient-schema.json
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
title: NotificationRecipient
---
