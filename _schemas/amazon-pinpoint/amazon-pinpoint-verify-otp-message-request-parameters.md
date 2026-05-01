---
description: Verify OTP message request.
layout: schema
name: VerifyOTPMessageRequestParameters
properties_list:
- description: ''
  name: DestinationIdentity
  type: object
- description: ''
  name: Otp
  type: object
- description: ''
  name: ReferenceId
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-verify-otp-message-request-parameters-schema.json
slug: amazon-pinpoint-verify-otp-message-request-parameters
source_filename: amazon-pinpoint-verify-otp-message-request-parameters-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-verify-otp-message-request-parameters-schema.json\",\n  \"title\": \"VerifyOTPMessageRequestParameters\",\n  \"description\": \"Verify OTP message request.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DestinationIdentity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The destination identity to send OTP to.\"\n        }\n      ]\n    },\n    \"Otp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The OTP the end user provided for verification.\"\n        }\n      ]\n    },\n    \"ReferenceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n     \
  \   },\n        {\n          \"description\": \"The reference identifier provided when the OTP was previously sent.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ReferenceId\",\n    \"Otp\",\n    \"DestinationIdentity\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-verify-otp-message-request-parameters-schema.json
tags:
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
title: VerifyOTPMessageRequestParameters
---
