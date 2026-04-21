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
