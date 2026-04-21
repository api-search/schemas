---
description: ConferenceMember schema from Bandwidth voice API
layout: schema
name: ConferenceMember
properties_list:
- description: The call ID of the conference member
  name: callId
  type: string
- description: The conference ID
  name: conferenceId
  type: string
- description: The URL for this member resource
  name: memberUrl
  type: string
- description: Whether the member is muted
  name: mute
  type: boolean
- description: Whether the member is on hold
  name: hold
  type: boolean
- description: List of call IDs that this member is coaching
  name: callIdsToCoach
  type: array
provider_name: Bandwidth
provider_slug: bandwidth
schema_file: json-schema/voice-conference-member-schema.json
slug: voice-conference-member
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
title: ConferenceMember
---
