---
description: Request to order phone numbers
layout: schema
name: OrderRequest
properties_list:
- description: A name for the order (required, max 50 characters)
  name: name
  type: string
- description: The site to assign the numbers to
  name: siteId
  type: string
- description: The SIP peer to assign the numbers to
  name: peerId
  type: string
- description: ''
  name: existingTelephoneNumberOrderType
  type: object
provider_name: Bandwidth
provider_slug: bandwidth
schema_file: json-schema/phone-numbers-order-request-schema.json
slug: phone-numbers-order-request
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
title: OrderRequest
---
