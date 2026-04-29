---
description: Verify OTP Message Response.
layout: schema
name: VerificationResponse
properties_list:
- description: ''
  name: Valid
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-verification-response-schema.json
slug: amazon-pinpoint-verification-response
source_filename: amazon-pinpoint-verification-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-verification-response-schema.json\",\n  \"title\": \"VerificationResponse\",\n  \"description\": \"Verify OTP Message Response.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Valid\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"description\": \"Specifies whether the OTP is valid or not.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-verification-response-schema.json
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
title: VerificationResponse
---
