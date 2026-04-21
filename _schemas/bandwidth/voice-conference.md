---
description: Conference schema from Bandwidth voice API
layout: schema
name: Conference
properties_list:
- description: The unique identifier for the conference
  name: id
  type: string
- description: The user-defined name of the conference
  name: name
  type: string
- description: The time the conference was created
  name: createdTime
  type: string
- description: The time the conference ended
  name: completedTime
  type: string
- description: Custom tag attached to the conference
  name: tag
  type: string
- description: List of currently active conference members
  name: activeMembers
  type: array
provider_name: Bandwidth
provider_slug: bandwidth
schema_file: json-schema/voice-conference-schema.json
slug: voice-conference
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
title: Conference
---
