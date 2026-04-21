---
description: MfaVerifyRequest schema from Bandwidth mfa API
layout: schema
name: MfaVerifyRequest
properties_list:
- description: The phone number the MFA code was sent to, in E.164 format
  name: to
  type: string
- description: The scope that was used when the code was generated. Must match for verification to succeed.
  name: scope
  type: string
- description: The MFA code entered by the user for verification
  name: code
  type: string
- description: The expiration window to check against, in minutes
  name: expirationTimeInMinutes
  type: number
provider_name: Bandwidth
provider_slug: bandwidth
schema_file: json-schema/mfa-mfa-verify-request-schema.json
slug: mfa-mfa-verify-request
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
title: MfaVerifyRequest
---
