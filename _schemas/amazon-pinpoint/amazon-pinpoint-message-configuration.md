---
description: Specifies the message configuration settings for a campaign.
layout: schema
name: MessageConfiguration
properties_list:
- description: ''
  name: ADMMessage
  type: object
- description: ''
  name: APNSMessage
  type: object
- description: ''
  name: BaiduMessage
  type: object
- description: ''
  name: CustomMessage
  type: object
- description: ''
  name: DefaultMessage
  type: object
- description: ''
  name: EmailMessage
  type: object
- description: ''
  name: GCMMessage
  type: object
- description: ''
  name: SMSMessage
  type: object
- description: ''
  name: InAppMessage
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-message-configuration-schema.json
slug: amazon-pinpoint-message-configuration
source_filename: amazon-pinpoint-message-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-message-configuration-schema.json\",\n  \"title\": \"MessageConfiguration\",\n  \"description\": \"Specifies the message configuration settings for a campaign.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ADMMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Message\"\n        },\n        {\n          \"description\": \"The message that the campaign sends through the ADM (Amazon Device Messaging) channel. If specified, this message overrides the default message.\"\n        }\n      ]\n    },\n    \"APNSMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Message\"\n        },\n        {\n          \"description\": \"The message that the campaign sends through the APNs (Apple Push Notification service) channel.\
  \ If specified, this message overrides the default message.\"\n        }\n      ]\n    },\n    \"BaiduMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Message\"\n        },\n        {\n          \"description\": \"The message that the campaign sends through the Baidu (Baidu Cloud Push) channel. If specified, this message overrides the default message.\"\n        }\n      ]\n    },\n    \"CustomMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CampaignCustomMessage\"\n        },\n        {\n          \"description\": \"<p>The message that the campaign sends through a custom channel, as specified by the delivery configuration (CustomDeliveryConfiguration) settings for the campaign. If specified, this message overrides the default message.</p> \"\n        }\n      ]\n    },\n    \"DefaultMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Message\"\n        },\n        {\n    \
  \      \"description\": \"The default message that the campaign sends through all the channels that are configured for the campaign.\"\n        }\n      ]\n    },\n    \"EmailMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CampaignEmailMessage\"\n        },\n        {\n          \"description\": \"The message that the campaign sends through the email channel. If specified, this message overrides the default message.\"\n        }\n      ]\n    },\n    \"GCMMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Message\"\n        },\n        {\n          \"description\": \"The message that the campaign sends through the GCM channel, which enables Amazon Pinpoint to send push notifications through the Firebase Cloud Messaging (FCM), formerly Google Cloud Messaging (GCM), service. If specified, this message overrides the default message.\"\n        }\n      ]\n    },\n    \"SMSMessage\": {\n      \"allOf\": [\n      \
  \  {\n          \"$ref\": \"#/components/schemas/CampaignSmsMessage\"\n        },\n        {\n          \"description\": \"The message that the campaign sends through the SMS channel. If specified, this message overrides the default message.\"\n        }\n      ]\n    },\n    \"InAppMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CampaignInAppMessage\"\n        },\n        {\n          \"description\": \"The in-app message configuration.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-message-configuration-schema.json
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
title: MessageConfiguration
---
