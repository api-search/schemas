---
description: Specifies the contents of an email message, composed of a subject, a text part, and an HTML part.
layout: schema
name: SimpleEmail
properties_list:
- description: ''
  name: HtmlPart
  type: object
- description: ''
  name: Subject
  type: object
- description: ''
  name: TextPart
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-simple-email-schema.json
slug: amazon-pinpoint-simple-email
source_filename: amazon-pinpoint-simple-email-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-simple-email-schema.json\",\n  \"title\": \"SimpleEmail\",\n  \"description\": \"Specifies the contents of an email message, composed of a subject, a text part, and an HTML part.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"HtmlPart\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SimpleEmailPart\"\n        },\n        {\n          \"description\": \"The body of the email message, in HTML format. We recommend using HTML format for email clients that render HTML content. You can include links, formatted text, and more in an HTML message.\"\n        }\n      ]\n    },\n    \"Subject\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SimpleEmailPart\"\n        },\n        {\n          \"description\": \"The subject line,\
  \ or title, of the email.\"\n        }\n      ]\n    },\n    \"TextPart\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SimpleEmailPart\"\n        },\n        {\n          \"description\": \"The body of the email message, in plain text format. We recommend using plain text format for email clients that don't render HTML content and clients that are connected to high-latency networks, such as mobile devices.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-simple-email-schema.json
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
title: SimpleEmail
---
