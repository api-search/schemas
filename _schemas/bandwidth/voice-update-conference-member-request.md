---
description: UpdateConferenceMemberRequest schema from Bandwidth voice API
layout: schema
name: UpdateConferenceMemberRequest
properties_list:
- description: Whether to mute the member
  name: mute
  type: boolean
- description: Whether to place the member on hold
  name: hold
  type: boolean
- description: List of call IDs that this member should coach
  name: callIdsToCoach
  type: array
provider_name: Bandwidth
provider_slug: bandwidth
schema_file: json-schema/voice-update-conference-member-request-schema.json
slug: voice-update-conference-member-request
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
title: UpdateConferenceMemberRequest
---
