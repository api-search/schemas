---
description: Represents a phone number managed through the Bandwidth Phone Numbers API, including its assignment, location metadata, and configured features.
layout: schema
name: Bandwidth Phone Number
properties_list:
- description: The full phone number, optionally in E.164 format
  name: fullNumber
  type: string
- description: The city associated with the phone number
  name: city
  type: string
- description: The two-letter state code associated with the phone number
  name: state
  type: string
- description: The Local Access and Transport Area (LATA) code
  name: lata
  type: string
- description: The rate center the phone number belongs to
  name: rateCenter
  type: string
- description: The current status of the phone number
  name: status
  type: string
- description: The site (sub-account) the number is assigned to
  name: siteId
  type: string
- description: The SIP peer (location) the number is assigned to
  name: sipPeerId
  type: string
- description: ''
  name: features
  type: object
provider_name: Bandwidth
provider_slug: bandwidth
schema_file: json-schema/bandwidth-phone-number-schema.json
slug: bandwidth-phone-number
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
title: Bandwidth Phone Number
---
