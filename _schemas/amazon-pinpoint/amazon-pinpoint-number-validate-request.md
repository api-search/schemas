---
description: Specifies a phone number to validate and retrieve information about.
layout: schema
name: NumberValidateRequest
properties_list:
- description: ''
  name: IsoCountryCode
  type: object
- description: ''
  name: PhoneNumber
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-number-validate-request-schema.json
slug: amazon-pinpoint-number-validate-request
source_filename: amazon-pinpoint-number-validate-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-number-validate-request-schema.json\",\n  \"title\": \"NumberValidateRequest\",\n  \"description\": \"Specifies a phone number to validate and retrieve information about.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"IsoCountryCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The two-character code, in ISO 3166-1 alpha-2 format, for the country or region where the phone number was originally registered.\"\n        }\n      ]\n    },\n    \"PhoneNumber\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The phone number to retrieve information about. The phone number that you provide should\
  \ include a valid numeric country code. Otherwise, the operation might result in an error.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-number-validate-request-schema.json
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
title: NumberValidateRequest
---
