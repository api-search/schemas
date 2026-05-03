---
description: Represents an individual error or transaction event in Sentry. Events are individual occurrences that get grouped into issues based on fingerprinting rules.
layout: schema
name: Sentry Event
properties_list:
- description: The unique identifier of the event.
  name: eventID
  type: string
- description: Additional context data attached to the event.
  name: context
  type: object
- description: When the event was created.
  name: dateCreated
  type: string
- description: When the event was received by Sentry.
  name: dateReceived
  type: string
- description: The structured data entries of the event (exception, request, breadcrumbs, etc.).
  name: entries
  type: array
- description: The event message.
  name: message
  type: string
- description: The title of the event.
  name: title
  type: string
- description: The platform that generated the event.
  name: platform
  type: string
- description: Tags associated with the event.
  name: tags
  type: array
- description: The type of event (e.g., error, default, transaction).
  name: type
  type: string
- description: The issue ID this event belongs to.
  name: groupID
  type: string
- description: Information about the SDK that captured the event.
  name: sdk
  type: object
- description: Information about the user who triggered the event.
  name: user
  type: object
- description: Structured context data (device, os, browser, runtime, etc.).
  name: contexts
  type: object
provider_name: Sentry
provider_slug: sentry-system
schema_file: json-schema/sentry-event-schema.json
slug: sentry-event
source_filename: sentry-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://sentry.io/schemas/event.json\",\n  \"title\": \"Sentry Event\",\n  \"description\": \"Represents an individual error or transaction event in Sentry. Events are individual occurrences that get grouped into issues based on fingerprinting rules.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"eventID\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the event.\"\n    },\n    \"context\": {\n      \"type\": \"object\",\n      \"description\": \"Additional context data attached to the event.\"\n    },\n    \"dateCreated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the event was created.\"\n    },\n    \"dateReceived\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the event was received by Sentry.\"\n    },\n    \"entries\": {\n      \"type\": \"\
  array\",\n      \"description\": \"The structured data entries of the event (exception, request, breadcrumbs, etc.).\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"type\": {\n            \"type\": \"string\",\n            \"description\": \"The type of entry (e.g., exception, request, breadcrumbs, message).\"\n          },\n          \"data\": {\n            \"type\": \"object\",\n            \"description\": \"The entry data, structure varies by type.\"\n          }\n        }\n      }\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"The event message.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The title of the event.\"\n    },\n    \"platform\": {\n      \"type\": \"string\",\n      \"description\": \"The platform that generated the event.\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"Tags associated with the event.\",\n      \"items\"\
  : {\n        \"type\": \"object\",\n        \"properties\": {\n          \"key\": {\n            \"type\": \"string\"\n          },\n          \"value\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of event (e.g., error, default, transaction).\"\n    },\n    \"groupID\": {\n      \"type\": \"string\",\n      \"description\": \"The issue ID this event belongs to.\"\n    },\n    \"sdk\": {\n      \"type\": \"object\",\n      \"description\": \"Information about the SDK that captured the event.\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\"\n        },\n        \"version\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"user\": {\n      \"type\": \"object\",\n      \"description\": \"Information about the user who triggered the event.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\"\n       \
  \ },\n        \"email\": {\n          \"type\": \"string\",\n          \"format\": \"email\"\n        },\n        \"username\": {\n          \"type\": \"string\"\n        },\n        \"ip_address\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"contexts\": {\n      \"type\": \"object\",\n      \"description\": \"Structured context data (device, os, browser, runtime, etc.).\",\n      \"properties\": {\n        \"device\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"name\": { \"type\": \"string\" },\n            \"family\": { \"type\": \"string\" },\n            \"model\": { \"type\": \"string\" },\n            \"arch\": { \"type\": \"string\" }\n          }\n        },\n        \"os\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"name\": { \"type\": \"string\" },\n            \"version\": { \"type\": \"string\" }\n          }\n        },\n        \"browser\": {\n          \"type\": \"object\",\n\
  \          \"properties\": {\n            \"name\": { \"type\": \"string\" },\n            \"version\": { \"type\": \"string\" }\n          }\n        },\n        \"runtime\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"name\": { \"type\": \"string\" },\n            \"version\": { \"type\": \"string\" }\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\"eventID\", \"dateCreated\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sentry-system/refs/heads/main/json-schema/sentry-event-schema.json
tags:
- APM
- Application Monitoring
- Bug Tracking
- Developer Tools
- Error Tracking
- Observability
- Performance Monitoring
- Real-Time Monitoring
title: Sentry Event
---
