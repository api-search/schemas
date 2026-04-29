---
description: Specifies the default settings and content for a message template that can be used in messages that are sent through a push notification channel.
layout: schema
name: DefaultPushNotificationTemplate
properties_list:
- description: ''
  name: Action
  type: object
- description: ''
  name: Body
  type: object
- description: ''
  name: Sound
  type: object
- description: ''
  name: Title
  type: object
- description: ''
  name: Url
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-default-push-notification-template-schema.json
slug: amazon-pinpoint-default-push-notification-template
source_filename: amazon-pinpoint-default-push-notification-template-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-default-push-notification-template-schema.json\",\n  \"title\": \"DefaultPushNotificationTemplate\",\n  \"description\": \"Specifies the default settings and content for a message template that can be used in messages that are sent through a push notification channel.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Action\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Action\"\n        },\n        {\n          \"description\": \"<p>The action to occur if a recipient taps a push notification that's based on the message template. Valid values are:</p> <ul><li><p>OPEN_APP - Your app opens or it becomes the foreground app if it was sent to the background. This is the default action.</p></li> <li><p>DEEP_LINK - Your app opens and displays a designated\
  \ user interface in the app. This setting uses the deep-linking features of the iOS and Android platforms.</p></li> <li><p>URL - The default mobile browser on the recipient's device opens and loads the web page at a URL that you specify.</p></li></ul>\"\n        }\n      ]\n    },\n    \"Body\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The message body to use in push notifications that are based on the message template.\"\n        }\n      ]\n    },\n    \"Sound\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"<p>The sound to play when a recipient receives a push notification that's based on the message template. You can use the default stream or specify the file name of a sound resource that's bundled in your app. On an Android platform, the sound file must reside in /res/raw/.</p> <p>For an iOS\
  \ platform, this value is the key for the name of a sound file in your app's main bundle or the Library/Sounds folder in your app's data container. If the sound file can't be found or you specify default for the value, the system plays the default alert sound.</p>\"\n        }\n      ]\n    },\n    \"Title\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The title to use in push notifications that are based on the message template. This title appears above the notification message on a recipient's device.\"\n        }\n      ]\n    },\n    \"Url\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The URL to open in a recipient's default mobile browser, if a recipient taps a push notification that's based on the message template and the value of the Action property is URL.\"\n        }\n      ]\n    }\n\
  \  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-default-push-notification-template-schema.json
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
title: DefaultPushNotificationTemplate
---
