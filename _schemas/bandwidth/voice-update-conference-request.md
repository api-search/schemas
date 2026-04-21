---
description: UpdateConferenceRequest schema from Bandwidth voice API
layout: schema
name: UpdateConferenceRequest
properties_list:
- description: Set to completed to end the conference and disconnect all members
  name: status
  type: string
- description: URL to redirect the conference to for new BXML instructions
  name: redirectUrl
  type: string
- description: The HTTP method for the redirect webhook
  name: redirectMethod
  type: string
- description: Custom tag for the conference
  name: tag
  type: string
provider_name: Bandwidth
provider_slug: bandwidth
schema_file: json-schema/voice-update-conference-request-schema.json
slug: voice-update-conference-request
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
title: UpdateConferenceRequest
---
