---
description: Specifies the settings and content for the default message and any default messages that you tailored for specific channels.
layout: schema
name: DirectMessageConfiguration
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
  name: DefaultMessage
  type: object
- description: ''
  name: DefaultPushNotificationMessage
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
  name: VoiceMessage
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-direct-message-configuration-schema.json
slug: amazon-pinpoint-direct-message-configuration
source_filename: amazon-pinpoint-direct-message-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-direct-message-configuration-schema.json\",\n  \"title\": \"DirectMessageConfiguration\",\n  \"description\": \"Specifies the settings and content for the default message and any default messages that you tailored for specific channels.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ADMMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ADMMessage\"\n        },\n        {\n          \"description\": \"The default push notification message for the ADM (Amazon Device Messaging) channel. This message overrides the default push notification message (DefaultPushNotificationMessage).\"\n        }\n      ]\n    },\n    \"APNSMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/APNSMessage\"\n        },\n        {\n\
  \          \"description\": \"The default push notification message for the APNs (Apple Push Notification service) channel. This message overrides the default push notification message (DefaultPushNotificationMessage).\"\n        }\n      ]\n    },\n    \"BaiduMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BaiduMessage\"\n        },\n        {\n          \"description\": \"The default push notification message for the Baidu (Baidu Cloud Push) channel. This message overrides the default push notification message (DefaultPushNotificationMessage).\"\n        }\n      ]\n    },\n    \"DefaultMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DefaultMessage\"\n        },\n        {\n          \"description\": \"The default message for all channels.\"\n        }\n      ]\n    },\n    \"DefaultPushNotificationMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DefaultPushNotificationMessage\"\
  \n        },\n        {\n          \"description\": \"The default push notification message for all push notification channels.\"\n        }\n      ]\n    },\n    \"EmailMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EmailMessage\"\n        },\n        {\n          \"description\": \"The default message for the email channel. This message overrides the default message (DefaultMessage).\"\n        }\n      ]\n    },\n    \"GCMMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GCMMessage\"\n        },\n        {\n          \"description\": \"The default push notification message for the GCM channel, which is used to send notifications through the Firebase Cloud Messaging (FCM), formerly Google Cloud Messaging (GCM), service. This message overrides the default push notification message (DefaultPushNotificationMessage).\"\n        }\n      ]\n    },\n    \"SMSMessage\": {\n      \"allOf\": [\n        {\n        \
  \  \"$ref\": \"#/components/schemas/SMSMessage\"\n        },\n        {\n          \"description\": \"The default message for the SMS channel. This message overrides the default message (DefaultMessage).\"\n        }\n      ]\n    },\n    \"VoiceMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VoiceMessage\"\n        },\n        {\n          \"description\": \"The default message for the voice channel. This message overrides the default message (DefaultMessage).\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-direct-message-configuration-schema.json
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
title: DirectMessageConfiguration
---
