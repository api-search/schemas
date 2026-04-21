---
description: A phone number assigned to the account
layout: schema
name: PhoneNumber
properties_list:
- description: The full phone number
  name: fullNumber
  type: string
- description: The city associated with the number
  name: city
  type: string
- description: The state associated with the number
  name: state
  type: string
- description: The LATA code
  name: lata
  type: string
- description: The rate center
  name: rateCenter
  type: string
- description: The current status of the number
  name: status
  type: string
- description: The site the number is assigned to
  name: siteId
  type: string
- description: The SIP peer the number is assigned to
  name: sipPeerId
  type: string
provider_name: Bandwidth
provider_slug: bandwidth
schema_file: json-schema/phone-numbers-phone-number-schema.json
slug: phone-numbers-phone-number
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
title: PhoneNumber
---
