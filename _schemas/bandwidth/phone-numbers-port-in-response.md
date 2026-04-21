---
description: Response containing port-in request details
layout: schema
name: PortInResponse
properties_list:
- description: The unique identifier for the port-in request
  name: portInId
  type: string
- description: The current status of the port-in request
  name: status
  type: string
- description: The requested FOC date
  name: requestedFocDate
  type: string
- description: The actual FOC date assigned by the carrier
  name: actualFocDate
  type: string
provider_name: Bandwidth
provider_slug: bandwidth
schema_file: json-schema/phone-numbers-port-in-response-schema.json
slug: phone-numbers-port-in-response
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
title: PortInResponse
---
