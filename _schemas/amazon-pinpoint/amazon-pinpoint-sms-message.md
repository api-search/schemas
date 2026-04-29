---
description: Specifies the default settings for a one-time SMS message that's sent directly to an endpoint.
layout: schema
name: SMSMessage
properties_list:
- description: ''
  name: Body
  type: object
- description: ''
  name: Keyword
  type: object
- description: ''
  name: MediaUrl
  type: object
- description: ''
  name: MessageType
  type: object
- description: ''
  name: OriginationNumber
  type: object
- description: ''
  name: SenderId
  type: object
- description: ''
  name: Substitutions
  type: object
- description: ''
  name: EntityId
  type: object
- description: ''
  name: TemplateId
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-sms-message-schema.json
slug: amazon-pinpoint-sms-message
source_filename: amazon-pinpoint-sms-message-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-sms-message-schema.json\",\n  \"title\": \"SMSMessage\",\n  \"description\": \"Specifies the default settings for a one-time SMS message that's sent directly to an endpoint.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Body\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The body of the SMS message.\"\n        }\n      ]\n    },\n    \"Keyword\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The SMS program name that you provided to AWS Support when you requested your dedicated number.\"\n        }\n      ]\n    },\n    \"MediaUrl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"\
  #/components/schemas/__string\"\n        },\n        {\n          \"description\": \"This field is reserved for future use.\"\n        }\n      ]\n    },\n    \"MessageType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MessageType\"\n        },\n        {\n          \"description\": \"The SMS message type. Valid values are TRANSACTIONAL (for messages that are critical or time-sensitive, such as a one-time passwords) and PROMOTIONAL (for messsages that aren't critical or time-sensitive, such as marketing messages).\"\n        }\n      ]\n    },\n    \"OriginationNumber\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The number to send the SMS message from. This value should be one of the dedicated long or short codes that's assigned to your AWS account. If you don't specify a long or short code, Amazon Pinpoint assigns a random long code to the SMS message and\
  \ sends the message from that code.\"\n        }\n      ]\n    },\n    \"SenderId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The sender ID to display as the sender of the message on a recipient's device. Support for sender IDs varies by country or region.\"\n        }\n      ]\n    },\n    \"Substitutions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MapOfListOf__string\"\n        },\n        {\n          \"description\": \"The message variables to use in the SMS message. You can override the default variables with individual address variables.\"\n        }\n      ]\n    },\n    \"EntityId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The entity ID or Principal Entity (PE) id received from the regulatory body for sending SMS in your country.\"\n        }\n\
  \      ]\n    },\n    \"TemplateId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The template ID received from the regulatory body for sending SMS in your country.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-sms-message-schema.json
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
title: SMSMessage
---
