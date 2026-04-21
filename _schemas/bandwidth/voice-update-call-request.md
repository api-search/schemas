---
description: UpdateCallRequest schema from Bandwidth voice API
layout: schema
name: UpdateCallRequest
properties_list:
- description: Set to completed to hang up the call
  name: state
  type: string
- description: The URL to redirect the call to for new BXML instructions
  name: redirectUrl
  type: string
- description: The HTTP method for the redirect webhook
  name: redirectMethod
  type: string
- description: Fallback URL if the primary redirect URL fails
  name: redirectFallbackUrl
  type: string
- description: The HTTP method for the fallback redirect webhook
  name: redirectFallbackMethod
  type: string
- description: A custom string to attach to the call for tracking purposes
  name: tag
  type: string
provider_name: Bandwidth
provider_slug: bandwidth
schema_file: json-schema/voice-update-call-request-schema.json
slug: voice-update-call-request
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
title: UpdateCallRequest
---
