---
description: Specifies the content and settings for a push notification that's sent to recipients of a campaign.
layout: schema
name: Message
properties_list:
- description: ''
  name: Action
  type: object
- description: ''
  name: Body
  type: object
- description: ''
  name: ImageIconUrl
  type: object
- description: ''
  name: ImageSmallIconUrl
  type: object
- description: ''
  name: ImageUrl
  type: object
- description: ''
  name: JsonBody
  type: object
- description: ''
  name: MediaUrl
  type: object
- description: ''
  name: RawContent
  type: object
- description: ''
  name: SilentPush
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
schema_file: json-schema/amazon-pinpoint-message-schema.json
slug: amazon-pinpoint-message
source_filename: amazon-pinpoint-message-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-message-schema.json\",\n  \"title\": \"Message\",\n  \"description\": \"Specifies the content and settings for a push notification that's sent to recipients of a campaign.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Action\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Action\"\n        },\n        {\n          \"description\": \"<p>The action to occur if a recipient taps the push notification. Valid values are:</p> <ul><li><p>OPEN_APP - Your app opens or it becomes the foreground app if it was sent to the background. This is the default action.</p></li> <li><p>DEEP_LINK - Your app opens and displays a designated user interface in the app. This setting uses the deep-linking features of iOS and Android.</p></li> <li><p>URL - The default mobile\
  \ browser on the recipient's device opens and loads the web page at a URL that you specify.</p></li></ul>\"\n        }\n      ]\n    },\n    \"Body\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The body of the notification message. The maximum number of characters is 200.\"\n        }\n      ]\n    },\n    \"ImageIconUrl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The URL of the image to display as the push-notification icon, such as the icon for the app.\"\n        }\n      ]\n    },\n    \"ImageSmallIconUrl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The URL of the image to display as the small, push-notification icon, such as a small version of the icon for the app.\"\n        }\n      ]\n\
  \    },\n    \"ImageUrl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The URL of an image to display in the push notification.\"\n        }\n      ]\n    },\n    \"JsonBody\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The JSON payload to use for a silent push notification.\"\n        }\n      ]\n    },\n    \"MediaUrl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The URL of the image or video to display in the push notification.\"\n        }\n      ]\n    },\n    \"RawContent\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The raw, JSON-formatted string to use as the payload for the notification message.\
  \ If specified, this value overrides all other content for the message.\"\n        }\n      ]\n    },\n    \"SilentPush\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"description\": \"Specifies whether the notification is a silent push notification, which is a push notification that doesn't display on a recipient's device. Silent push notifications can be used for cases such as updating an app's configuration, displaying messages in an in-app message center, or supporting phone home functionality.\"\n        }\n      ]\n    },\n    \"TimeToLive\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"description\": \"<p>The number of seconds that the push-notification service should keep the message, if the service is unable to deliver the notification the first time. This value is converted to an expiration value when it's sent to a push-notification\
  \ service. If this value is 0, the service treats the notification as if it expires immediately and the service doesn't store or try to deliver the notification again.</p> <p>This value doesn't apply to messages that are sent through the Amazon Device Messaging (ADM) service.</p>\"\n        }\n      ]\n    },\n    \"Title\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The title to display above the notification message on a recipient's device.\"\n        }\n      ]\n    },\n    \"Url\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The URL to open in a recipient's default mobile browser, if a recipient taps the push notification and the value of the Action property is URL.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-message-schema.json
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
title: Message
---
