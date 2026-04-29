---
description: Represents an SMS or MMS message sent or received through the Bandwidth Messaging API, including delivery status, media attachments, and routing metadata.
layout: schema
name: Bandwidth Message
properties_list:
- description: The unique identifier for the message, assigned by Bandwidth
  name: id
  type: string
- description: The Bandwidth phone number that owns the message
  name: owner
  type: string
- description: The Bandwidth application ID associated with the message
  name: applicationId
  type: string
- description: The source phone number in E.164 format
  name: from
  type: string
- description: Array of destination phone numbers in E.164 format
  name: to
  type: array
- description: The text content of the message
  name: text
  type: string
- description: Array of media URLs for MMS attachments
  name: media
  type: array
- description: The direction of the message (in for received, out for sent)
  name: direction
  type: string
- description: The number of segments the message was split into for delivery
  name: segmentCount
  type: integer
- description: The ISO 8601 timestamp when the message was created
  name: time
  type: string
- description: A custom string attached to the message for tracking
  name: tag
  type: string
- description: The priority level of the message
  name: priority
  type: string
- description: The expiration time after which undelivered messages are discarded
  name: expiration
  type: string
provider_name: Bandwidth
provider_slug: bandwidth
schema_file: json-schema/bandwidth-message-schema.json
slug: bandwidth-message
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.com/schemas/bandwidth/message.json\",\n  \"title\": \"Bandwidth Message\",\n  \"description\": \"Represents an SMS or MMS message sent or received through the Bandwidth Messaging API, including delivery status, media attachments, and routing metadata.\",\n  \"type\": \"object\",\n  \"required\": [\"from\", \"to\", \"applicationId\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the message, assigned by Bandwidth\"\n    },\n    \"owner\": {\n      \"type\": \"string\",\n      \"description\": \"The Bandwidth phone number that owns the message\"\n    },\n    \"applicationId\": {\n      \"type\": \"string\",\n      \"description\": \"The Bandwidth application ID associated with the message\"\n    },\n    \"from\": {\n      \"type\": \"string\",\n      \"pattern\": \"^\\\\+1[2-9]\\\\d{9}$\",\n      \"description\"\
  : \"The source phone number in E.164 format\"\n    },\n    \"to\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"pattern\": \"^\\\\+1[2-9]\\\\d{9}$\"\n      },\n      \"minItems\": 1,\n      \"maxItems\": 50,\n      \"description\": \"Array of destination phone numbers in E.164 format\"\n    },\n    \"text\": {\n      \"type\": \"string\",\n      \"maxLength\": 2048,\n      \"description\": \"The text content of the message\"\n    },\n    \"media\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"format\": \"uri\"\n      },\n      \"description\": \"Array of media URLs for MMS attachments\"\n    },\n    \"direction\": {\n      \"type\": \"string\",\n      \"enum\": [\"in\", \"out\"],\n      \"description\": \"The direction of the message (in for received, out for sent)\"\n    },\n    \"segmentCount\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"description\": \"The number of segments\
  \ the message was split into for delivery\"\n    },\n    \"time\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The ISO 8601 timestamp when the message was created\"\n    },\n    \"tag\": {\n      \"type\": \"string\",\n      \"description\": \"A custom string attached to the message for tracking\"\n    },\n    \"priority\": {\n      \"type\": \"string\",\n      \"enum\": [\"default\", \"high\"],\n      \"default\": \"default\",\n      \"description\": \"The priority level of the message\"\n    },\n    \"expiration\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The expiration time after which undelivered messages are discarded\"\n    }\n  },\n  \"$defs\": {\n    \"MessageDeliveryEvent\": {\n      \"type\": \"object\",\n      \"description\": \"A webhook event for message delivery status updates\",\n      \"required\": [\"type\", \"time\"],\n      \"properties\": {\n        \"type\": {\n       \
  \   \"type\": \"string\",\n          \"enum\": [\"message-received\", \"message-delivered\", \"message-failed\", \"message-sending\"],\n          \"description\": \"The type of messaging event\"\n        },\n        \"time\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The timestamp of the event\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"A human-readable description of the event\"\n        },\n        \"to\": {\n          \"type\": \"string\",\n          \"description\": \"The destination phone number\"\n        },\n        \"errorCode\": {\n          \"type\": \"integer\",\n          \"description\": \"The Bandwidth error code for failed messages\"\n        },\n        \"message\": {\n          \"type\": \"object\",\n          \"description\": \"The message associated with this event\",\n          \"properties\": {\n            \"id\": {\n              \"type\": \"\
  string\",\n              \"description\": \"The message identifier\"\n            },\n            \"direction\": {\n              \"type\": \"string\",\n              \"enum\": [\"in\", \"out\"],\n              \"description\": \"The message direction\"\n            },\n            \"segmentCount\": {\n              \"type\": \"integer\",\n              \"description\": \"Number of message segments\"\n            }\n          }\n        }\n      }\n    },\n    \"Media\": {\n      \"type\": \"object\",\n      \"description\": \"A media file stored in Bandwidth for MMS messaging\",\n      \"properties\": {\n        \"mediaName\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the media file\"\n        },\n        \"contentLength\": {\n          \"type\": \"integer\",\n          \"maximum\": 3932160,\n          \"description\": \"The size of the media file in bytes (max 3.75 MB)\"\n        },\n        \"contentType\": {\n          \"type\": \"string\",\n    \
  \      \"description\": \"The MIME type of the media file\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/bandwidth-message-schema.json
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
title: Bandwidth Message
---
