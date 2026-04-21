---
description: An E911 endpoint representing an end user
layout: schema
name: Endpoint
properties_list:
- description: The unique identifier for the endpoint
  name: endpointId
  type: string
- description: The Alternate End User ID (AEUI) that identifies the end user
  name: alternateEndUserId
  type: string
- description: The name of the end user for PSAP display
  name: callerName
  type: string
- description: The ID of the validated location associated with this endpoint
  name: locationId
  type: string
- description: The phone number associated with this endpoint
  name: telephoneNumber
  type: string
- description: Whether the endpoint is currently active
  name: activated
  type: boolean
provider_name: Bandwidth
provider_slug: bandwidth
schema_file: json-schema/emergency-calling-endpoint-schema.json
slug: emergency-calling-endpoint
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
title: Endpoint
---
