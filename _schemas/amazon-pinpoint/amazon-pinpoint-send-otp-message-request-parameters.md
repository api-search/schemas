---
description: Send OTP message request parameters.
layout: schema
name: SendOTPMessageRequestParameters
properties_list:
- description: ''
  name: AllowedAttempts
  type: object
- description: ''
  name: BrandName
  type: object
- description: ''
  name: Channel
  type: object
- description: ''
  name: CodeLength
  type: object
- description: ''
  name: DestinationIdentity
  type: object
- description: ''
  name: EntityId
  type: object
- description: ''
  name: Language
  type: object
- description: ''
  name: OriginationIdentity
  type: object
- description: ''
  name: ReferenceId
  type: object
- description: ''
  name: TemplateId
  type: object
- description: ''
  name: ValidityPeriod
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-send-otp-message-request-parameters-schema.json
slug: amazon-pinpoint-send-otp-message-request-parameters
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-send-otp-message-request-parameters-schema.json\",\n  \"title\": \"SendOTPMessageRequestParameters\",\n  \"description\": \"Send OTP message request parameters.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AllowedAttempts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"description\": \"The attempts allowed to validate an OTP.\"\n        }\n      ]\n    },\n    \"BrandName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The brand name that will be substituted into the OTP message body. Should be owned by calling AWS account.\"\n        }\n      ]\n    },\n    \"Channel\": {\n      \"allOf\": [\n        {\n\
  \          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"Channel type for the OTP message. Supported values: [SMS].\"\n        }\n      ]\n    },\n    \"CodeLength\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"description\": \"The number of characters in the generated OTP.\"\n        }\n      ]\n    },\n    \"DestinationIdentity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The destination identity to send OTP to.\"\n        }\n      ]\n    },\n    \"EntityId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"A unique Entity ID received from DLT after entity registration is approved.\"\n        }\n      ]\n    },\n    \"Language\": {\n      \"allOf\": [\n        {\n \
  \         \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The language to be used for the outgoing message body containing the OTP.\"\n        }\n      ]\n    },\n    \"OriginationIdentity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The origination identity used to send OTP from.\"\n        }\n      ]\n    },\n    \"ReferenceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"Developer-specified reference identifier. Required to match during OTP verification.\"\n        }\n      ]\n    },\n    \"TemplateId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"A unique Template ID received from DLT after entity registration is approved.\"\n        }\n      ]\n\
  \    },\n    \"ValidityPeriod\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"description\": \"The time in minutes before the OTP is no longer valid.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"BrandName\",\n    \"ReferenceId\",\n    \"Channel\",\n    \"DestinationIdentity\",\n    \"OriginationIdentity\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-send-otp-message-request-parameters-schema.json
tags:
- AWS
- Campaigns
- Communications
- Email
- Marketing
- Messaging
- Push Notifications
- SMS
- Voice
- Customer Engagement
- Segmentation
- Journeys
- Analytics
title: SendOTPMessageRequestParameters
---
