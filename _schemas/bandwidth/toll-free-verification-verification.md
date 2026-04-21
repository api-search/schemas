---
description: Verification schema from Bandwidth toll-free-verification API
layout: schema
name: Verification
properties_list:
- description: The unique identifier for the verification request
  name: verificationId
  type: string
- description: The toll-free numbers associated with this verification
  name: telephoneNumbers
  type: array
- description: The current verification status
  name: status
  type: string
- description: The business name on the verification
  name: businessName
  type: string
- description: The messaging use case
  name: useCase
  type: string
- description: The date and time the verification was submitted
  name: submissionDate
  type: string
- description: The date and time the verification was approved or denied
  name: verificationDate
  type: string
- description: The reason for denial, if the verification was denied
  name: denialReason
  type: string
provider_name: Bandwidth
provider_slug: bandwidth
schema_file: json-schema/toll-free-verification-verification-schema.json
slug: toll-free-verification-verification
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
title: Verification
---
