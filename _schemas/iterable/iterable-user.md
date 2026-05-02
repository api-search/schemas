---
description: A user profile in the Iterable marketing automation platform. Users are the primary audience for campaigns and represent contacts that can receive messages across email, push, SMS, and in-app channels.
layout: schema
name: Iterable User
properties_list:
- description: The primary email address of the user, used as the default unique identifier
  name: email
  type: string
- description: An alternative unique identifier for the user, set by the integrating application
  name: userId
  type: string
- description: ISO 8601 timestamp of when the user was first created in Iterable
  name: signupDate
  type: string
- description: ISO 8601 timestamp of the most recent profile update
  name: profileUpdatedAt
  type: string
- description: Custom data fields stored on the user profile, used for segmentation and personalization
  name: dataFields
  type: object
- description: Phone number in E.164 format for SMS messaging
  name: phoneNumber
  type: string
- description: IDs of the email lists the user is subscribed to
  name: emailListIds
  type: array
- description: IDs of channels the user has unsubscribed from
  name: unsubscribedChannelIds
  type: array
- description: IDs of message types the user has unsubscribed from
  name: unsubscribedMessageTypeIds
  type: array
- description: Mobile and web devices registered to the user for push notifications
  name: devices
  type: array
provider_name: Iterable
provider_slug: iterable
schema_file: json-schema/iterable-user-schema.json
slug: iterable-user
source_filename: iterable-user-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemas.api-evangelist.com/schemas/iterable/user.json\",\n  \"title\": \"Iterable User\",\n  \"description\": \"A user profile in the Iterable marketing automation platform. Users are the primary audience for campaigns and represent contacts that can receive messages across email, push, SMS, and in-app channels.\",\n  \"type\": \"object\",\n  \"required\": [\"email\"],\n  \"properties\": {\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"The primary email address of the user, used as the default unique identifier\"\n    },\n    \"userId\": {\n      \"type\": \"string\",\n      \"description\": \"An alternative unique identifier for the user, set by the integrating application\"\n    },\n    \"signupDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp of when the user was\
  \ first created in Iterable\"\n    },\n    \"profileUpdatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp of the most recent profile update\"\n    },\n    \"dataFields\": {\n      \"type\": \"object\",\n      \"description\": \"Custom data fields stored on the user profile, used for segmentation and personalization\",\n      \"additionalProperties\": true\n    },\n    \"phoneNumber\": {\n      \"type\": \"string\",\n      \"pattern\": \"^\\\\+?[1-9]\\\\d{1,14}$\",\n      \"description\": \"Phone number in E.164 format for SMS messaging\"\n    },\n    \"emailListIds\": {\n      \"type\": \"array\",\n      \"description\": \"IDs of the email lists the user is subscribed to\",\n      \"items\": {\n        \"type\": \"integer\"\n      }\n    },\n    \"unsubscribedChannelIds\": {\n      \"type\": \"array\",\n      \"description\": \"IDs of channels the user has unsubscribed from\",\n      \"items\": {\n        \"type\": \"\
  integer\"\n      }\n    },\n    \"unsubscribedMessageTypeIds\": {\n      \"type\": \"array\",\n      \"description\": \"IDs of message types the user has unsubscribed from\",\n      \"items\": {\n        \"type\": \"integer\"\n      }\n    },\n    \"devices\": {\n      \"type\": \"array\",\n      \"description\": \"Mobile and web devices registered to the user for push notifications\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Device\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"Device\": {\n      \"type\": \"object\",\n      \"description\": \"A device registered for push notifications\",\n      \"required\": [\"token\", \"platform\"],\n      \"properties\": {\n        \"token\": {\n          \"type\": \"string\",\n          \"description\": \"The device push token (APNs or FCM)\"\n        },\n        \"platform\": {\n          \"type\": \"string\",\n          \"enum\": [\"APNS\", \"APNS_SANDBOX\", \"GCM\"],\n          \"description\": \"The push notification platform\"\n    \
  \    },\n        \"applicationName\": {\n          \"type\": \"string\",\n          \"description\": \"The registered application name\"\n        },\n        \"endpointEnabled\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the push endpoint is currently active\"\n        },\n        \"dataFields\": {\n          \"type\": \"object\",\n          \"description\": \"Custom data fields associated with the device\",\n          \"additionalProperties\": true\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/iterable/refs/heads/main/json-schema/iterable-user-schema.json
tags:
- Cross-Channel Messaging
- Customer Engagement
- Email
- Marketing Automation
- Push Notifications
- SMS
title: Iterable User
---
