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
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/toll-free-verification-verification-request-schema.json\",\n  \"title\": \"VerificationRequest\",\n  \"description\": \"VerificationRequest schema from Bandwidth toll-free-verification API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"telephoneNumbers\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"List of toll-free numbers to verify in E.164 format\",\n      \"example\": [\n        \"+18005551234\"\n      ]\n    },\n    \"businessName\": {\n      \"type\": \"string\",\n      \"description\": \"The legal name of the business sending messages from the toll-free number\"\n    },\n    \"businessContact\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"firstName\",\n        \"lastName\",\n        \"email\",\n     \
  \   \"phone\"\n      ],\n      \"properties\": {\n        \"firstName\": {\n          \"type\": \"string\",\n          \"description\": \"First name of the business contact\"\n        },\n        \"lastName\": {\n          \"type\": \"string\",\n          \"description\": \"Last name of the business contact\"\n        },\n        \"email\": {\n          \"type\": \"string\",\n          \"format\": \"email\",\n          \"description\": \"Email address of the business contact\"\n        },\n        \"phone\": {\n          \"type\": \"string\",\n          \"description\": \"Phone number of the business contact\"\n        }\n      }\n    },\n    \"businessWebsite\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The business website URL\"\n    },\n    \"messageVolume\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"10\",\n        \"100\",\n        \"1,000\",\n        \"10,000\",\n        \"100,000\",\n        \"250,000\",\n        \"500,000\"\
  ,\n        \"750,000\",\n        \"1,000,000+\"\n      ],\n      \"description\": \"Estimated monthly message volume\"\n    },\n    \"useCase\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"TWO_FACTOR_AUTHENTICATION\",\n        \"APP_NOTIFICATIONS\",\n        \"ACCOUNT_NOTIFICATIONS\",\n        \"CUSTOMER_CARE\",\n        \"DELIVERY_NOTIFICATIONS\",\n        \"FRAUD_ALERT_MESSAGING\",\n        \"HIGHER_EDUCATION\",\n        \"MARKETING\",\n        \"POLLING_AND_VOTING\",\n        \"PUBLIC_SERVICE_ANNOUNCEMENT\",\n        \"SECURITY_ALERT\"\n      ],\n      \"description\": \"The primary use case for messaging from this toll-free number\"\n    },\n    \"useCaseSummary\": {\n      \"type\": \"string\",\n      \"maxLength\": 500,\n      \"description\": \"A detailed description of how the toll-free number will be used for messaging (max 500 characters)\"\n    },\n    \"messageContent\": {\n      \"type\": \"string\",\n      \"maxLength\": 1000,\n      \"description\": \"Sample\
  \ message content that will be sent from the number\"\n    },\n    \"optInWorkflow\": {\n      \"type\": \"string\",\n      \"maxLength\": 500,\n      \"description\": \"Description of how recipients opt in to receive messages\"\n    },\n    \"optInWorkflowImageUrls\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"format\": \"uri\"\n      },\n      \"description\": \"URLs to images showing the opt-in workflow (screenshots)\"\n    },\n    \"additionalInformation\": {\n      \"type\": \"string\",\n      \"maxLength\": 500,\n      \"description\": \"Any additional information to support the verification request\"\n    }\n  },\n  \"required\": [\n    \"telephoneNumbers\",\n    \"businessName\",\n    \"businessContact\",\n    \"messageVolume\",\n    \"useCase\",\n    \"useCaseSummary\",\n    \"optInWorkflow\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/toll-free-verification-verification-request-schema.json
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
