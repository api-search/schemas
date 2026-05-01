---
description: Schema for a Firebase Cloud Messaging (FCM) HTTP v1 API send request, used to deliver push notifications and data messages to devices.
layout: schema
name: Firebase Cloud Messaging Message
properties_list:
- description: The message to send
  name: message
  type: object
- description: If true, the message is validated but not sent
  name: validate_only
  type: boolean
provider_name: Google Firebase
provider_slug: google-firebase
schema_file: json-schema/google-firebase-fcm-message-schema.json
slug: google-firebase-fcm-message
source_filename: google-firebase-fcm-message-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://firebase.google.com/schemas/fcm/message.json\",\n  \"title\": \"Firebase Cloud Messaging Message\",\n  \"description\": \"Schema for a Firebase Cloud Messaging (FCM) HTTP v1 API send request, used to deliver push notifications and data messages to devices.\",\n  \"type\": \"object\",\n  \"required\": [\"message\"],\n  \"properties\": {\n    \"message\": {\n      \"type\": \"object\",\n      \"description\": \"The message to send\",\n      \"properties\": {\n        \"token\": {\n          \"type\": \"string\",\n          \"description\": \"Registration token of the target device\"\n        },\n        \"topic\": {\n          \"type\": \"string\",\n          \"description\": \"Topic name to send the message to\"\n        },\n        \"condition\": {\n          \"type\": \"string\",\n          \"description\": \"Condition expression for targeting multiple topics\"\n        },\n        \"\
  notification\": {\n          \"$ref\": \"#/$defs/Notification\"\n        },\n        \"data\": {\n          \"type\": \"object\",\n          \"additionalProperties\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"Arbitrary key-value payload delivered to the client app\"\n        },\n        \"android\": {\n          \"$ref\": \"#/$defs/AndroidConfig\"\n        },\n        \"webpush\": {\n          \"$ref\": \"#/$defs/WebpushConfig\"\n        },\n        \"apns\": {\n          \"$ref\": \"#/$defs/ApnsConfig\"\n        }\n      }\n    },\n    \"validate_only\": {\n      \"type\": \"boolean\",\n      \"description\": \"If true, the message is validated but not sent\",\n      \"default\": false\n    }\n  },\n  \"$defs\": {\n    \"Notification\": {\n      \"type\": \"object\",\n      \"description\": \"Basic notification template\",\n      \"properties\": {\n        \"title\": {\n          \"type\": \"string\",\n          \"description\": \"The notification\
  \ title\"\n        },\n        \"body\": {\n          \"type\": \"string\",\n          \"description\": \"The notification body text\"\n        },\n        \"image\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL of an image to display in the notification\"\n        }\n      }\n    },\n    \"AndroidConfig\": {\n      \"type\": \"object\",\n      \"description\": \"Android-specific message configuration\",\n      \"properties\": {\n        \"priority\": {\n          \"type\": \"string\",\n          \"enum\": [\"NORMAL\", \"HIGH\"]\n        },\n        \"ttl\": {\n          \"type\": \"string\",\n          \"description\": \"Message time-to-live as a duration string (e.g. 3600s)\"\n        },\n        \"collapse_key\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"WebpushConfig\": {\n      \"type\": \"object\",\n      \"description\": \"Web push-specific message configuration\",\n      \"properties\": {\n     \
  \   \"headers\": {\n          \"type\": \"object\",\n          \"additionalProperties\": { \"type\": \"string\" }\n        }\n      }\n    },\n    \"ApnsConfig\": {\n      \"type\": \"object\",\n      \"description\": \"Apple Push Notification Service configuration\",\n      \"properties\": {\n        \"headers\": {\n          \"type\": \"object\",\n          \"additionalProperties\": { \"type\": \"string\" }\n        },\n        \"payload\": {\n          \"type\": \"object\",\n          \"additionalProperties\": true\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-firebase/refs/heads/main/json-schema/google-firebase-fcm-message-schema.json
tags:
- Analytics
- Authentication
- Backend as a Service
- Cloud Messaging
- Google Cloud
- Hosting
- Mobile
- Real-Time Database
title: Firebase Cloud Messaging Message
---
