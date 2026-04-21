---
description: MessageList schema from Bandwidth messaging API
layout: schema
name: MessageList
properties_list:
- description: The total number of messages matching the query
  name: totalCount
  type: integer
- description: ''
  name: pageInfo
  type: object
- description: ''
  name: messages
  type: array
provider_name: Bandwidth
provider_slug: bandwidth
schema_file: json-schema/messaging-message-list-schema.json
slug: messaging-message-list
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
title: MessageList
---
