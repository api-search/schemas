---
description: Specifies the content and settings for an SMS message that's sent to recipients of a campaign.
layout: schema
name: CampaignSmsMessage
properties_list:
- description: ''
  name: Body
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
  name: EntityId
  type: object
- description: ''
  name: TemplateId
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-campaign-sms-message-schema.json
slug: amazon-pinpoint-campaign-sms-message
source_filename: amazon-pinpoint-campaign-sms-message-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-campaign-sms-message-schema.json\",\n  \"title\": \"CampaignSmsMessage\",\n  \"description\": \"Specifies the content and settings for an SMS message that's sent to recipients of a campaign.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Body\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The body of the SMS message.\"\n        }\n      ]\n    },\n    \"MessageType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MessageType\"\n        },\n        {\n          \"description\": \"The SMS message type. Valid values are TRANSACTIONAL (for messages that are critical or time-sensitive, such as a one-time passwords) and PROMOTIONAL (for messsages that aren't\
  \ critical or time-sensitive, such as marketing messages).\"\n        }\n      ]\n    },\n    \"OriginationNumber\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The long code to send the SMS message from. This value should be one of the dedicated long codes that's assigned to your AWS account. Although it isn't required, we recommend that you specify the long code using an E.164 format to ensure prompt and accurate delivery of the message. For example, +12065550100.\"\n        }\n      ]\n    },\n    \"SenderId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The sender ID to display on recipients' devices when they receive the SMS message.\"\n        }\n      ]\n    },\n    \"EntityId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n\
  \          \"description\": \"The entity ID or Principal Entity (PE) id received from the regulatory body for sending SMS in your country.\"\n        }\n      ]\n    },\n    \"TemplateId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The template ID received from the regulatory body for sending SMS in your country.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-campaign-sms-message-schema.json
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
title: CampaignSmsMessage
---
