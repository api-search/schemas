---
description: Provides information about the content and settings for a message template that can be used in messages that are sent through a push notification channel.
layout: schema
name: PushNotificationTemplateResponse
properties_list:
- description: ''
  name: ADM
  type: object
- description: ''
  name: APNS
  type: object
- description: ''
  name: Arn
  type: object
- description: ''
  name: Baidu
  type: object
- description: ''
  name: CreationDate
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
  name: LastModifiedDate
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
- description: ''
  name: TemplateName
  type: object
- description: ''
  name: TemplateType
  type: object
- description: ''
  name: Version
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-push-notification-template-response-schema.json
slug: amazon-pinpoint-push-notification-template-response
source_filename: amazon-pinpoint-push-notification-template-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-push-notification-template-response-schema.json\",\n  \"title\": \"PushNotificationTemplateResponse\",\n  \"description\": \"Provides information about the content and settings for a message template that can be used in messages that are sent through a push notification channel.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ADM\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AndroidPushNotificationTemplate\"\n        },\n        {\n          \"description\": \"The message template that's used for the ADM (Amazon Device Messaging) channel. This message template overrides the default template for push notification channels (DefaultPushNotificationTemplate).\"\n        }\n      ]\n    },\n    \"APNS\": {\n      \"allOf\": [\n        {\n          \"\
  $ref\": \"#/components/schemas/APNSPushNotificationTemplate\"\n        },\n        {\n          \"description\": \"The message template that's used for the APNs (Apple Push Notification service) channel. This message template overrides the default template for push notification channels (DefaultPushNotificationTemplate).\"\n        }\n      ]\n    },\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the message template.\"\n        }\n      ]\n    },\n    \"Baidu\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AndroidPushNotificationTemplate\"\n        },\n        {\n          \"description\": \"The message template that's used for the Baidu (Baidu Cloud Push) channel. This message template overrides the default template for push notification channels (DefaultPushNotificationTemplate).\"\n        }\n      ]\n    },\n\
  \    \"CreationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The date, in ISO 8601 format, when the message template was created.\"\n        }\n      ]\n    },\n    \"Default\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DefaultPushNotificationTemplate\"\n        },\n        {\n          \"description\": \"The default message template that's used for push notification channels.\"\n        }\n      ]\n    },\n    \"DefaultSubstitutions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The JSON object that specifies the default values that are used for message variables in the message template. This object is a set of key-value pairs. Each key defines a message variable in the template. The corresponding value defines the default value for that variable.\"\n  \
  \      }\n      ]\n    },\n    \"GCM\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AndroidPushNotificationTemplate\"\n        },\n        {\n          \"description\": \"The message template that's used for the GCM channel, which is used to send notifications through the Firebase Cloud Messaging (FCM), formerly Google Cloud Messaging (GCM), service. This message template overrides the default template for push notification channels (DefaultPushNotificationTemplate).\"\n        }\n      ]\n    },\n    \"LastModifiedDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The date, in ISO 8601 format, when the message template was last modified.\"\n        }\n      ]\n    },\n    \"RecommenderId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for the\
  \ recommender model that's used by the message template.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MapOf__string\"\n        },\n        {\n          \"description\": \"A string-to-string map of key-value pairs that identifies the tags that are associated with the message template. Each tag consists of a required tag key and an associated tag value.\"\n        }\n      ]\n    },\n    \"TemplateDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The custom description of the message template.\"\n        }\n      ]\n    },\n    \"TemplateName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The name of the message template.\"\n        }\n      ]\n    },\n    \"TemplateType\": {\n      \"allOf\": [\n        {\n    \
  \      \"$ref\": \"#/components/schemas/TemplateType\"\n        },\n        {\n          \"description\": \"The type of channel that the message template is designed for. For a push notification template, this value is PUSH.\"\n        }\n      ]\n    },\n    \"Version\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier, as an integer, for the active version of the message template, or the version of the template that you specified by using the version parameter in your request.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"LastModifiedDate\",\n    \"CreationDate\",\n    \"TemplateType\",\n    \"TemplateName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-push-notification-template-response-schema.json
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
title: PushNotificationTemplateResponse
---
