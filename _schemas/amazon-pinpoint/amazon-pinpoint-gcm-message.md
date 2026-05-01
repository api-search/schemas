---
description: Specifies the settings for a one-time message that's sent directly to an endpoint through the GCM channel. The GCM channel enables Amazon Pinpoint to send messages to the Firebase Cloud Messaging (FCM), formerly Google Cloud Messaging (GCM), service.
layout: schema
name: GCMMessage
properties_list:
- description: ''
  name: Action
  type: object
- description: ''
  name: Body
  type: object
- description: ''
  name: CollapseKey
  type: object
- description: ''
  name: Data
  type: object
- description: ''
  name: IconReference
  type: object
- description: ''
  name: ImageIconUrl
  type: object
- description: ''
  name: ImageUrl
  type: object
- description: ''
  name: Priority
  type: object
- description: ''
  name: RawContent
  type: object
- description: ''
  name: RestrictedPackageName
  type: object
- description: ''
  name: SilentPush
  type: object
- description: ''
  name: SmallImageIconUrl
  type: object
- description: ''
  name: Sound
  type: object
- description: ''
  name: Substitutions
  type: object
- description: ''
  name: TimeToLive
  type: object
- description: ''
  name: Title
  type: object
- description: ''
  name: Url
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-gcm-message-schema.json
slug: amazon-pinpoint-gcm-message
source_filename: amazon-pinpoint-gcm-message-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-gcm-message-schema.json\",\n  \"title\": \"GCMMessage\",\n  \"description\": \"Specifies the settings for a one-time message that's sent directly to an endpoint through the GCM channel. The GCM channel enables Amazon Pinpoint to send messages to the Firebase Cloud Messaging (FCM), formerly Google Cloud Messaging (GCM), service.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Action\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Action\"\n        },\n        {\n          \"description\": \"<p>The action to occur if the recipient taps the push notification. Valid values are:</p> <ul><li><p>OPEN_APP - Your app opens or it becomes the foreground app if it was sent to the background. This is the default action.</p></li> <li><p>DEEP_LINK - Your app opens\
  \ and displays a designated user interface in the app. This action uses the deep-linking features of the Android platform.</p></li> <li><p>URL - The default mobile browser on the recipient's device opens and loads the web page at a URL that you specify.</p></li></ul>\"\n        }\n      ]\n    },\n    \"Body\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The body of the notification message.\"\n        }\n      ]\n    },\n    \"CollapseKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"<p>An arbitrary string that identifies a group of messages that can be collapsed to ensure that only the last message is sent when delivery can resume. This helps avoid sending too many instances of the same messages when the recipient's device comes online again or becomes active.</p> <p>Amazon Pinpoint specifies\
  \ this value in the Firebase Cloud Messaging (FCM) collapse_key parameter when it sends the notification message to FCM.</p>\"\n        }\n      ]\n    },\n    \"Data\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MapOf__string\"\n        },\n        {\n          \"description\": \"The JSON data payload to use for the push notification, if the notification is a silent push notification. This payload is added to the data.pinpoint.jsonBody object of the notification.\"\n        }\n      ]\n    },\n    \"IconReference\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The icon image name of the asset saved in your app.\"\n        }\n      ]\n    },\n    \"ImageIconUrl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The URL of the large icon image to display in the content\
  \ view of the push notification.\"\n        }\n      ]\n    },\n    \"ImageUrl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The URL of an image to display in the push notification.\"\n        }\n      ]\n    },\n    \"Priority\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"<p>para>normal - The notification might be delayed. Delivery is optimized for battery usage on the recipient's device. Use this value unless immediate delivery is required.</p>/listitem> <li><p>high - The notification is sent immediately and might wake a sleeping device.</p></li>/para> <p>Amazon Pinpoint specifies this value in the FCM priority parameter when it sends the notification message to FCM.</p> <p>The equivalent values for Apple Push Notification service (APNs) are 5, for normal, and 10, for high. If you specify an\
  \ APNs value for this property, Amazon Pinpoint accepts and converts the value to the corresponding FCM value.</p>\"\n        }\n      ]\n    },\n    \"RawContent\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The raw, JSON-formatted string to use as the payload for the notification message. If specified, this value overrides all other content for the message.\"\n        }\n      ]\n    },\n    \"RestrictedPackageName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The package name of the application where registration tokens must match in order for the recipient to receive the message.\"\n        }\n      ]\n    },\n    \"SilentPush\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"description\": \"Specifies whether the\
  \ notification is a silent push notification, which is a push notification that doesn't display on a recipient's device. Silent push notifications can be used for cases such as updating an app's configuration or supporting phone home functionality.\"\n        }\n      ]\n    },\n    \"SmallImageIconUrl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The URL of the small icon image to display in the status bar and the content view of the push notification.\"\n        }\n      ]\n    },\n    \"Sound\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The sound to play when the recipient receives the push notification. You can use the default stream or specify the file name of a sound resource that's bundled in your app. On an Android platform, the sound file must reside in /res/raw/.\"\n        }\n    \
  \  ]\n    },\n    \"Substitutions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MapOfListOf__string\"\n        },\n        {\n          \"description\": \"The default message variables to use in the notification message. You can override the default variables with individual address variables.\"\n        }\n      ]\n    },\n    \"TimeToLive\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"description\": \"<p>The amount of time, in seconds, that FCM should store and attempt to deliver the push notification, if the service is unable to deliver the notification the first time. If you don't specify this value, FCM defaults to the maximum value, which is 2,419,200 seconds (28 days).</p> <p>Amazon Pinpoint specifies this value in the FCM time_to_live parameter when it sends the notification message to FCM.</p>\"\n        }\n      ]\n    },\n    \"Title\": {\n      \"allOf\": [\n \
  \       {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The title to display above the notification message on the recipient's device.\"\n        }\n      ]\n    },\n    \"Url\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The URL to open in the recipient's default mobile browser, if a recipient taps the push notification and the value of the Action property is URL.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-gcm-message-schema.json
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
title: GCMMessage
---
