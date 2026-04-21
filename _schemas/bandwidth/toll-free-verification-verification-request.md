---
description: VerificationRequest schema from Bandwidth toll-free-verification API
layout: schema
name: VerificationRequest
properties_list:
- description: List of toll-free numbers to verify in E.164 format
  name: telephoneNumbers
  type: array
- description: The legal name of the business sending messages from the toll-free number
  name: businessName
  type: string
- description: ''
  name: businessContact
  type: object
- description: The business website URL
  name: businessWebsite
  type: string
- description: Estimated monthly message volume
  name: messageVolume
  type: string
- description: The primary use case for messaging from this toll-free number
  name: useCase
  type: string
- description: A detailed description of how the toll-free number will be used for messaging (max 500 characters)
  name: useCaseSummary
  type: string
- description: Sample message content that will be sent from the number
  name: messageContent
  type: string
- description: Description of how recipients opt in to receive messages
  name: optInWorkflow
  type: string
- description: URLs to images showing the opt-in workflow (screenshots)
  name: optInWorkflowImageUrls
  type: array
- description: Any additional information to support the verification request
  name: additionalInformation
  type: string
provider_name: Bandwidth
provider_slug: bandwidth
schema_file: json-schema/toll-free-verification-verification-request-schema.json
slug: toll-free-verification-verification-request
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
title: VerificationRequest
---
