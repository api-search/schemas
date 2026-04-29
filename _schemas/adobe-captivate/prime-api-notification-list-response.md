---
description: Paginated list of notifications
layout: schema
name: NotificationListResponse
properties_list:
- description: ''
  name: data
  type: array
- description: Pagination links following JSON:API conventions
  name: links
  type: object
provider_name: Adobe Captivate
provider_slug: adobe-captivate
schema_file: json-schema/prime-api-notification-list-response-schema.json
slug: prime-api-notification-list-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/json-schema/prime-api-notification-list-response-schema.json\",\n  \"title\": \"NotificationListResponse\",\n  \"description\": \"Paginated list of notifications\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"A user notification\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"Unique notification identifier\"\n          },\n          \"type\": {\n            \"type\": \"string\",\n            \"const\": \"userNotification\"\n          },\n          \"attributes\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"actionTaken\": {\n                \"type\": \"boolean\",\n                \"\
  description\": \"Whether the user has acted on this notification\"\n              },\n              \"channel\": {\n                \"type\": \"string\",\n                \"description\": \"Notification delivery channel\"\n              },\n              \"dateCreated\": {\n                \"type\": \"string\",\n                \"format\": \"date-time\",\n                \"description\": \"Notification creation timestamp\"\n              },\n              \"message\": {\n                \"type\": \"object\",\n                \"description\": \"Notification message content\"\n              },\n              \"modelType\": {\n                \"type\": \"string\",\n                \"description\": \"The type of model this notification relates to\"\n              },\n              \"read\": {\n                \"type\": \"boolean\",\n                \"description\": \"Whether the notification has been read\"\n              }\n            }\n          }\n        }\n      }\n    },\n    \"links\"\
  : {\n      \"type\": \"object\",\n      \"description\": \"Pagination links following JSON:API conventions\",\n      \"properties\": {\n        \"self\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL for the current page\"\n        },\n        \"next\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL for the next page\"\n        },\n        \"prev\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL for the previous page\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/json-schema/prime-api-notification-list-response-schema.json
tags:
- Authoring
- Education
- eLearning
- LMS
- SCORM
- Training
- xAPI
title: NotificationListResponse
---
