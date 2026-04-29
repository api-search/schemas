---
description: Specifies the content and settings for a message template that can be used in messages that are sent through a push notification channel.
layout: schema
name: PushNotificationTemplateRequest
properties_list:
- description: ''
  name: ADM
  type: object
- description: ''
  name: APNS
  type: object
- description: ''
  name: Baidu
  type: object
- description: ''
  name: Default
  type: object
- description: ''
  name: DefaultSubstitutions
  type: object
- description: ''
  name: GCM
  type: object
- description: ''
  name: RecommenderId
  type: object
- description: ''
  name: tags
  type: object
- description: ''
  name: TemplateDescription
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-push-notification-template-request-schema.json
slug: amazon-pinpoint-push-notification-template-request
source_filename: amazon-pinpoint-push-notification-template-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-push-notification-template-request-schema.json\",\n  \"title\": \"PushNotificationTemplateRequest\",\n  \"description\": \"Specifies the content and settings for a message template that can be used in messages that are sent through a push notification channel.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ADM\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AndroidPushNotificationTemplate\"\n        },\n        {\n          \"description\": \"The message template to use for the ADM (Amazon Device Messaging) channel. This message template overrides the default template for push notification channels (DefaultPushNotificationTemplate).\"\n        }\n      ]\n    },\n    \"APNS\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/APNSPushNotificationTemplate\"\
  \n        },\n        {\n          \"description\": \"The message template to use for the APNs (Apple Push Notification service) channel. This message template overrides the default template for push notification channels (DefaultPushNotificationTemplate).\"\n        }\n      ]\n    },\n    \"Baidu\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AndroidPushNotificationTemplate\"\n        },\n        {\n          \"description\": \"The message template to use for the Baidu (Baidu Cloud Push) channel. This message template overrides the default template for push notification channels (DefaultPushNotificationTemplate).\"\n        }\n      ]\n    },\n    \"Default\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DefaultPushNotificationTemplate\"\n        },\n        {\n          \"description\": \"The default message template to use for push notification channels.\"\n        }\n      ]\n    },\n    \"DefaultSubstitutions\": {\n\
  \      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"A JSON object that specifies the default values to use for message variables in the message template. This object is a set of key-value pairs. Each key defines a message variable in the template. The corresponding value defines the default value for that variable. When you create a message that's based on the template, you can override these defaults with message-specific and address-specific variables and values.\"\n        }\n      ]\n    },\n    \"GCM\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AndroidPushNotificationTemplate\"\n        },\n        {\n          \"description\": \"The message template to use for the GCM channel, which is used to send notifications through the Firebase Cloud Messaging (FCM), formerly Google Cloud Messaging (GCM), service. This message template overrides the default template for push\
  \ notification channels (DefaultPushNotificationTemplate).\"\n        }\n      ]\n    },\n    \"RecommenderId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for the recommender model to use for the message template. Amazon Pinpoint uses this value to determine how to retrieve and process data from a recommender model when it sends messages that use the template, if the template contains message variables for recommendation data.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MapOf__string\"\n        },\n        {\n          \"description\": \"A string-to-string map of key-value pairs that defines the tags to associate with the message template. Each tag consists of a required tag key and an associated tag value.\"\n        }\n      ]\n    },\n    \"TemplateDescription\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"A custom description of the message template.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-push-notification-template-request-schema.json
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
title: PushNotificationTemplateRequest
---
