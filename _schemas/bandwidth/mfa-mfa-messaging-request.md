---
description: MfaMessagingRequest schema from Bandwidth mfa API
layout: schema
name: MfaMessagingRequest
properties_list:
- description: The Bandwidth phone number to send the SMS from, in E.164 format
  name: from
  type: string
- description: The destination phone number to send the MFA code to, in E.164 format
  name: to
  type: string
- description: The ID of the Bandwidth messaging application to use for sending the SMS
  name: applicationId
  type: string
- description: An optional field to denote what scope or action the MFA code is for. This is returned during verification.
  name: scope
  type: string
- description: The message template to send. Use {CODE} as a placeholder for the generated MFA code.
  name: message
  type: string
- description: The number of digits in the generated MFA code (4-8)
  name: digits
  type: integer
- description: The time in minutes before the MFA code expires (1-15, default 3 minutes)
  name: expirationTimeInMinutes
  type: number
provider_name: Bandwidth
provider_slug: bandwidth
schema_file: json-schema/mfa-mfa-messaging-request-schema.json
slug: mfa-mfa-messaging-request
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
title: MfaMessagingRequest
---
