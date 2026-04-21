---
description: Error schema from Bandwidth messaging API
layout: schema
name: Error
properties_list:
- description: The error type identifier
  name: type
  type: string
- description: A human-readable description of the error
  name: description
  type: string
- description: ''
  name: fieldErrors
  type: array
provider_name: Bandwidth
provider_slug: bandwidth
schema_file: json-schema/messaging-error-schema.json
slug: messaging-error
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
title: Error
---
