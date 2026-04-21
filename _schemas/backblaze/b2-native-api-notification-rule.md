---
description: NotificationRule schema from Backblaze B2 Native API
layout: schema
name: NotificationRule
properties_list:
- description: Name for this notification rule
  name: name
  type: string
- description: Event types that trigger this notification
  name: eventTypes
  type: array
- description: Whether this rule is enabled
  name: isEnabled
  type: boolean
- description: ''
  name: targetConfiguration
  type: object
provider_name: Backblaze
provider_slug: backblaze
schema_file: json-schema/b2-native-api-notification-rule-schema.json
slug: b2-native-api-notification-rule
tags:
- Cloud Storage
- Object Storage
- Storage
- Backup
title: NotificationRule
---
