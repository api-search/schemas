---
description: A notification about an event or a task.
layout: schema
name: Notification
properties_list:
- description: The notification progress.
  name: progress
  type: integer
- description: ''
  name: user
  type: object
- description: The notification unique identifier.
  name: uuid
  type: string
- description: The notification name.
  name: name
  type: string
- description: The operation title.
  name: title
  type: string
- description: The notification description.
  name: description
  type: string
- description: The time that this notification was created.
  name: created_at
  type: string
- description: The time that the task or event this notification is tracking was started at.
  name: started_at
  type: string
- description: The time that the task or event this notification is tracking was completed at.
  name: completed_at
  type: string
- description: The status of the notification.
  name: status
  type: string
- description: The notification type.
  name: type
  type: string
- description: A collection of metadata related to the notification.
  name: metadata
  type: object
- description: ''
  name: labels
  type: object
- description: ''
  name: _links
  type: object
provider_name: Acquia
provider_slug: acquia
schema_file: json-schema/acquia-cloud-notification-schema.json
slug: acquia-cloud-notification
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/acquia/refs/heads/main/json-schema/acquia-cloud-notification-schema.json\",\n  \"title\": \"Notification\",\n  \"description\": \"A notification about an event or a task.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"progress\": {\n      \"type\": \"integer\",\n      \"description\": \"The notification progress.\",\n      \"minimum\": 0,\n      \"maximum\": 100\n    },\n    \"user\": {\n      \"$ref\": \"#/components/schemas/Acquia_Cloud_API_Documentation_user-stub\"\n    },\n    \"uuid\": {\n      \"type\": \"string\",\n      \"description\": \"The notification unique identifier.\",\n      \"format\": \"uuid\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The notification name.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The operation title.\"\n    },\n    \"description\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"The notification description.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time that this notification was created.\"\n    },\n    \"started_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time that the task or event this notification is tracking was started at.\"\n    },\n    \"completed_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time that the task or event this notification is tracking was completed at.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the notification.\",\n      \"enum\": [\n        \"completed\",\n        \"in-progress\",\n        \"failed\"\n      ]\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The notification type.\",\n      \"enum\":\
  \ [\n        \"task\",\n        \"event\"\n      ]\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"description\": \"A collection of metadata related to the notification.\",\n      \"properties\": {\n        \"environments\": {\n          \"$ref\": \"#/components/schemas/Acquia_Cloud_API_Documentation_environment-metadata\"\n        }\n      }\n    },\n    \"labels\": {\n      \"$ref\": \"#/components/schemas/Acquia_Cloud_API_Documentation_notification-labels\"\n    },\n    \"_links\": {\n      \"$ref\": \"#/components/schemas/Acquia_Cloud_API_Documentation_links\"\n    }\n  },\n  \"required\": [\n    \"progress\",\n    \"user\",\n    \"uuid\",\n    \"name\",\n    \"title\",\n    \"description\",\n    \"created_at\",\n    \"started_at\",\n    \"completed_at\",\n    \"status\",\n    \"type\",\n    \"metadata\",\n    \"labels\",\n    \"_links\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acquia/refs/heads/main/json-schema/acquia-cloud-notification-schema.json
tags:
- Content
- Experience
title: Notification
---
