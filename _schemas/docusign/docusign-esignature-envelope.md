---
description: Contains the properties of an envelope.
layout: schema
name: Envelope
properties_list:
- description: The unique identifier of the envelope.
  name: envelopeId
  type: string
- description: The URI for retrieving the envelope.
  name: envelopeUri
  type: string
- description: Current status of the envelope.
  name: status
  type: string
- description: The date and time the status last changed.
  name: statusChangedDateTime
  type: string
- description: The subject line of the envelope email.
  name: emailSubject
  type: string
- description: The body text of the envelope email.
  name: emailBlurb
  type: string
- description: The date and time the envelope was created.
  name: createdDateTime
  type: string
- description: The date and time the envelope was sent.
  name: sentDateTime
  type: string
- description: The date and time the envelope was delivered.
  name: deliveredDateTime
  type: string
- description: The date and time the envelope was completed.
  name: completedDateTime
  type: string
- description: The date and time the envelope was voided.
  name: voidedDateTime
  type: string
- description: The reason the envelope was voided.
  name: voidedReason
  type: string
- description: The date and time the envelope was declined.
  name: declinedDateTime
  type: string
- description: ''
  name: documents
  type: array
- description: Purge state of the envelope.
  name: purgeState
  type: string
- description: The ID of the brand applied to the envelope.
  name: brandId
  type: string
- description: URI for retrieving the certificate of completion.
  name: certificateUri
  type: string
- description: Whether this envelope uses a signature provider.
  name: isSignatureProviderEnvelope
  type: string
- description: The signing location. Valid values are inPerson and online.
  name: signingLocation
  type: string
- description: Whether the envelope expiration is enabled.
  name: expireEnabled
  type: string
- description: The date and time the envelope expires.
  name: expireDateTime
  type: string
- description: Number of days after which the envelope expires.
  name: expireAfter
  type: string
- description: Whether auto-navigation is enabled for recipients.
  name: autoNavigation
  type: string
- description: Reserved for DocuSign use.
  name: anySigner
  type: string
provider_name: Docusign
provider_slug: docusign
schema_file: json-schema/docusign-esignature-envelope-schema.json
slug: docusign-esignature-envelope
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Envelope\",\n  \"type\": \"object\",\n  \"description\": \"Contains the properties of an envelope.\",\n  \"properties\": {\n    \"envelopeId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the envelope.\"\n    },\n    \"envelopeUri\": {\n      \"type\": \"string\",\n      \"description\": \"The URI for retrieving the envelope.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current status of the envelope.\"\n    },\n    \"statusChangedDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the status last changed.\"\n    },\n    \"emailSubject\": {\n      \"type\": \"string\",\n      \"description\": \"The subject line of the envelope email.\"\n    },\n    \"emailBlurb\": {\n      \"type\": \"string\",\n      \"description\": \"The body text of the envelope email.\"\n    },\n    \"createdDateTime\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"The date and time the envelope was created.\"\n    },\n    \"sentDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the envelope was sent.\"\n    },\n    \"deliveredDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the envelope was delivered.\"\n    },\n    \"completedDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the envelope was completed.\"\n    },\n    \"voidedDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the envelope was voided.\"\n    },\n    \"voidedReason\": {\n      \"type\": \"string\",\n      \"description\": \"The reason the envelope was voided.\"\n    },\n    \"declinedDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the envelope was declined.\"\n    },\n    \"documents\": {\n      \"type\": \"array\"\n    },\n    \"purgeState\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Purge state of the envelope.\"\n    },\n    \"brandId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the brand applied to the envelope.\"\n    },\n    \"certificateUri\": {\n      \"type\": \"string\",\n      \"description\": \"URI for retrieving the certificate of completion.\"\n    },\n    \"isSignatureProviderEnvelope\": {\n      \"type\": \"string\",\n      \"description\": \"Whether this envelope uses a signature provider.\"\n    },\n    \"signingLocation\": {\n      \"type\": \"string\",\n      \"description\": \"The signing location. Valid values are inPerson and online.\"\n    },\n    \"expireEnabled\": {\n      \"type\": \"string\",\n      \"description\": \"Whether the envelope expiration is enabled.\"\n    },\n    \"expireDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the envelope expires.\"\n    },\n    \"expireAfter\": {\n      \"type\": \"string\",\n \
  \     \"description\": \"Number of days after which the envelope expires.\"\n    },\n    \"autoNavigation\": {\n      \"type\": \"string\",\n      \"description\": \"Whether auto-navigation is enabled for recipients.\"\n    },\n    \"anySigner\": {\n      \"type\": \"string\",\n      \"description\": \"Reserved for DocuSign use.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/docusign/refs/heads/main/json-schema/docusign-esignature-envelope-schema.json
tags:
- Agreements
- Contracts
- Digital Transaction Management
- Documents
- Electronic Signatures
- eSignature
title: Envelope
---
