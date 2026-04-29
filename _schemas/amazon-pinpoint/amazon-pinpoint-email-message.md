---
description: Specifies the default settings and content for a one-time email message that's sent directly to an endpoint.
layout: schema
name: EmailMessage
properties_list:
- description: ''
  name: Body
  type: object
- description: ''
  name: FeedbackForwardingAddress
  type: object
- description: ''
  name: FromAddress
  type: object
- description: ''
  name: RawEmail
  type: object
- description: ''
  name: ReplyToAddresses
  type: object
- description: ''
  name: SimpleEmail
  type: object
- description: ''
  name: Substitutions
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-email-message-schema.json
slug: amazon-pinpoint-email-message
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-email-message-schema.json\",\n  \"title\": \"EmailMessage\",\n  \"description\": \"Specifies the default settings and content for a one-time email message that's sent directly to an endpoint.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Body\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The body of the email message.\"\n        }\n      ]\n    },\n    \"FeedbackForwardingAddress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The email address to forward bounces and complaints to, if feedback forwarding is enabled.\"\n        }\n      ]\n    },\n    \"FromAddress\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The verified email address to send the email message from. The default value is the FromAddress specified for the email channel.\"\n        }\n      ]\n    },\n    \"RawEmail\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RawEmail\"\n        },\n        {\n          \"description\": \"The email message, represented as a raw MIME message.\"\n        }\n      ]\n    },\n    \"ReplyToAddresses\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListOf__string\"\n        },\n        {\n          \"description\": \"The reply-to email address(es) for the email message. If a recipient replies to the email, each reply-to address receives the reply.\"\n        }\n      ]\n    },\n    \"SimpleEmail\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SimpleEmail\"\n        },\n        {\n\
  \          \"description\": \"The email message, composed of a subject, a text part, and an HTML part.\"\n        }\n      ]\n    },\n    \"Substitutions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MapOfListOf__string\"\n        },\n        {\n          \"description\": \"The default message variables to use in the email message. You can override the default variables with individual address variables.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-email-message-schema.json
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
title: EmailMessage
---
