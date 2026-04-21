---
description: An available phone number from Bandwidth inventory
layout: schema
name: AvailableNumber
properties_list:
- description: The full phone number in E.164 format
  name: fullNumber
  type: string
- description: The city associated with the number
  name: city
  type: string
- description: The state associated with the number
  name: state
  type: string
- description: The LATA code for the number
  name: lata
  type: string
- description: The rate center for the number
  name: rateCenter
  type: string
provider_name: Bandwidth
provider_slug: bandwidth
schema_file: json-schema/phone-numbers-available-number-schema.json
slug: phone-numbers-available-number
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
title: AvailableNumber
---
