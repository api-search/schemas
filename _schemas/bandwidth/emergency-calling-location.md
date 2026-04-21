---
description: A validated physical location for E911 emergency routing
layout: schema
name: Location
properties_list:
- description: The unique identifier for the location
  name: locationId
  type: string
- description: A description of the location
  name: description
  type: string
- description: ''
  name: address
  type: object
- description: The validation status of the location
  name: status
  type: string
- description: The latitude coordinate of the location
  name: latitude
  type: number
- description: The longitude coordinate of the location
  name: longitude
  type: number
provider_name: Bandwidth
provider_slug: bandwidth
schema_file: json-schema/emergency-calling-location-schema.json
slug: emergency-calling-location
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
title: Location
---
