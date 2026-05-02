---
description: A service communication message from the Office 365 Service Communications API representing an incident, planned maintenance, or Message Center communication.
layout: schema
name: Message
properties_list:
- description: The message identifier.
  name: Id
  type: string
- description: The message name.
  name: Name
  type: string
- description: The title of the message.
  name: Title
  type:
  - string
  - 'null'
- description: The start time of the event.
  name: StartTime
  type: string
- description: The end time of the event.
  name: EndTime
  type: string
- description: The current status of the event.
  name: Status
  type: string
- description: History of messages published for this event.
  name: Messages
  type: array
- description: The last time the message was updated.
  name: LastUpdatedTime
  type: string
- description: The workload associated with the message.
  name: Workload
  type: string
- description: The display name of the workload.
  name: WorkloadDisplayName
  type: string
- description: The feature associated with the message.
  name: Feature
  type: string
- description: The display name of the feature.
  name: FeatureDisplayName
  type: string
- description: The type of message.
  name: MessageType
  type: string
provider_name: Microsoft Office Integration
provider_slug: microsoft-office-integration
schema_file: json-schema/message.json
slug: message
source_filename: message.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"message.json\",\n  \"title\": \"Message\",\n  \"description\": \"A service communication message from the Office 365 Service Communications API representing an incident, planned maintenance, or Message Center communication.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"The message identifier.\"\n    },\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"The message name.\"\n    },\n    \"Title\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The title of the message.\"\n    },\n    \"StartTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The start time of the event.\"\n    },\n    \"EndTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The end time of the event.\"\n    },\n    \"Status\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"The current status of the event.\"\n    },\n    \"Messages\": {\n      \"type\": \"array\",\n      \"description\": \"History of messages published for this event.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"PublishedTime\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\",\n            \"description\": \"The time the message was published.\"\n          },\n          \"MessageText\": {\n            \"type\": \"string\",\n            \"description\": \"The text content of the message.\"\n          }\n        },\n        \"required\": [\"PublishedTime\", \"MessageText\"]\n      }\n    },\n    \"LastUpdatedTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The last time the message was updated.\"\n    },\n    \"Workload\": {\n      \"type\": \"string\",\n      \"description\": \"The workload associated with\
  \ the message.\"\n    },\n    \"WorkloadDisplayName\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the workload.\"\n    },\n    \"Feature\": {\n      \"type\": \"string\",\n      \"description\": \"The feature associated with the message.\"\n    },\n    \"FeatureDisplayName\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the feature.\"\n    },\n    \"MessageType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of message.\",\n      \"enum\": [\"Incident\", \"PlannedMaintenance\", \"MessageCenter\"]\n    }\n  },\n  \"required\": [\"Id\", \"StartTime\", \"Status\", \"Messages\", \"LastUpdatedTime\"]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-office-integration/refs/heads/main/json-schema/message.json
tags:
- Microsoft 365
- Microsoft Office Integration
- Office 365
title: Message
---
