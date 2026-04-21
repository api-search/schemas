---
description: Request to port phone numbers from another carrier
layout: schema
name: PortInRequest
properties_list:
- description: The site to assign ported numbers to
  name: siteId
  type: string
- description: The SIP peer to assign ported numbers to
  name: peerId
  type: string
- description: The billing telephone number for the account being ported
  name: billingTelephoneNumber
  type: string
- description: ''
  name: subscriber
  type: object
- description: The name of the current carrier
  name: losingCarrierName
  type: string
- description: List of phone numbers to port
  name: listOfPhoneNumbers
  type: array
- description: Requested Firm Order Commitment date
  name: requestedFocDate
  type: string
provider_name: Bandwidth
provider_slug: bandwidth
schema_file: json-schema/phone-numbers-port-in-request-schema.json
slug: phone-numbers-port-in-request
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
title: PortInRequest
---
