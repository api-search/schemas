---
description: Specifies the contents of an email message, represented as a raw MIME message.
layout: schema
name: RawEmail
properties_list:
- description: ''
  name: Data
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-raw-email-schema.json
slug: amazon-pinpoint-raw-email
source_filename: amazon-pinpoint-raw-email-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-raw-email-schema.json\",\n  \"title\": \"RawEmail\",\n  \"description\": \"Specifies the contents of an email message, represented as a raw MIME message.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Data\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__blob\"\n        },\n        {\n          \"description\": \"The email message, represented as a raw MIME message. The entire message must be base64 encoded.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-raw-email-schema.json
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
title: RawEmail
---
