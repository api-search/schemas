---
description: Response containing a list of notification recipients
layout: schema
name: NotificationRecipientListResponse
properties_list:
- description: ''
  name: notificationRecipients
  type: array
provider_name: Bandwidth
provider_slug: bandwidth
schema_file: json-schema/emergency-calling-notification-recipient-list-response-schema.json
slug: emergency-calling-notification-recipient-list-response
source_filename: emergency-calling-notification-recipient-list-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/emergency-calling-notification-recipient-list-response-schema.json\",\n  \"title\": \"NotificationRecipientListResponse\",\n  \"description\": \"Response containing a list of notification recipients\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"notificationRecipients\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/NotificationRecipient\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/emergency-calling-notification-recipient-list-response-schema.json
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
title: NotificationRecipientListResponse
---
