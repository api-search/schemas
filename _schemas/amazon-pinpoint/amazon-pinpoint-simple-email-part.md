---
description: Specifies the subject or body of an email message, represented as textual email data and the applicable character set.
layout: schema
name: SimpleEmailPart
properties_list:
- description: ''
  name: Charset
  type: object
- description: ''
  name: Data
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-simple-email-part-schema.json
slug: amazon-pinpoint-simple-email-part
source_filename: amazon-pinpoint-simple-email-part-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-simple-email-part-schema.json\",\n  \"title\": \"SimpleEmailPart\",\n  \"description\": \"Specifies the subject or body of an email message, represented as textual email data and the applicable character set.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Charset\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The applicable character set for the message content.\"\n        }\n      ]\n    },\n    \"Data\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The textual data of the message content.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-simple-email-part-schema.json
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
title: SimpleEmailPart
---
