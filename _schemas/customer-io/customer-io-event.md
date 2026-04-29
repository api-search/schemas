---
description: An event in Customer.io representing a customer action or behavior tracked via the Track API or Pipelines API. Events are used to trigger campaigns, build segments, and personalize messages.
layout: schema
name: Customer.io Event
properties_list:
- description: The event name describing the action the customer took.
  name: name
  type: string
- description: The event type. Standard events have no type specified. Use page for page view events.
  name: type
  type: string
- description: Custom data associated with the event. Any key-value pairs included are available for use in campaigns, segments, and message personalization.
  name: data
  type: object
- description: A UNIX timestamp of when the event occurred. If not provided, the current time is used.
  name: timestamp
  type: integer
- description: An anonymous identifier for events not yet associated with a known customer. Used for anonymous event tracking and later merging.
  name: anonymous_id
  type: string
- description: The customer identifier the event is associated with.
  name: customer_id
  type: string
- description: ''
  name: context
  type: object
provider_name: Customer.io
provider_slug: customer-io
schema_file: json-schema/customer-io-event-schema.json
slug: customer-io-event
source_filename: customer-io-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://customer.io/schemas/customer-io/event.json\",\n  \"title\": \"Customer.io Event\",\n  \"description\": \"An event in Customer.io representing a customer action or behavior tracked via the Track API or Pipelines API. Events are used to trigger campaigns, build segments, and personalize messages.\",\n  \"type\": \"object\",\n  \"required\": [\"name\"],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The event name describing the action the customer took.\",\n      \"minLength\": 1,\n      \"maxLength\": 255\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The event type. Standard events have no type specified. Use page for page view events.\",\n      \"enum\": [\"page\", \"screen\", \"event\"]\n    },\n    \"data\": {\n      \"type\": \"object\",\n      \"description\": \"Custom data associated with the event. Any\
  \ key-value pairs included are available for use in campaigns, segments, and message personalization.\",\n      \"additionalProperties\": true\n    },\n    \"timestamp\": {\n      \"type\": \"integer\",\n      \"description\": \"A UNIX timestamp of when the event occurred. If not provided, the current time is used.\"\n    },\n    \"anonymous_id\": {\n      \"type\": \"string\",\n      \"description\": \"An anonymous identifier for events not yet associated with a known customer. Used for anonymous event tracking and later merging.\"\n    },\n    \"customer_id\": {\n      \"type\": \"string\",\n      \"description\": \"The customer identifier the event is associated with.\"\n    },\n    \"context\": {\n      \"$ref\": \"#/$defs/EventContext\"\n    }\n  },\n  \"$defs\": {\n    \"EventContext\": {\n      \"type\": \"object\",\n      \"description\": \"Contextual information about the event including device, location, and library details.\",\n      \"properties\": {\n        \"ip\": {\n  \
  \        \"type\": \"string\",\n          \"description\": \"The IP address of the user when the event occurred.\",\n          \"format\": \"ipv4\"\n        },\n        \"locale\": {\n          \"type\": \"string\",\n          \"description\": \"The locale of the user.\",\n          \"pattern\": \"^[a-z]{2}(-[A-Z]{2})?$\"\n        },\n        \"timezone\": {\n          \"type\": \"string\",\n          \"description\": \"The IANA timezone of the user.\"\n        },\n        \"user_agent\": {\n          \"type\": \"string\",\n          \"description\": \"The user agent string from the browser or device.\"\n        },\n        \"page\": {\n          \"type\": \"object\",\n          \"description\": \"Page context for web events.\",\n          \"properties\": {\n            \"url\": {\n              \"type\": \"string\",\n              \"format\": \"uri\",\n              \"description\": \"The full page URL.\"\n            },\n            \"title\": {\n              \"type\": \"string\",\n\
  \              \"description\": \"The page title.\"\n            },\n            \"referrer\": {\n              \"type\": \"string\",\n              \"format\": \"uri\",\n              \"description\": \"The referring page URL.\"\n            },\n            \"path\": {\n              \"type\": \"string\",\n              \"description\": \"The URL path.\"\n            }\n          }\n        },\n        \"device\": {\n          \"type\": \"object\",\n          \"description\": \"Device context for mobile events.\",\n          \"properties\": {\n            \"id\": {\n              \"type\": \"string\",\n              \"description\": \"The device identifier.\"\n            },\n            \"manufacturer\": {\n              \"type\": \"string\",\n              \"description\": \"The device manufacturer.\"\n            },\n            \"model\": {\n              \"type\": \"string\",\n              \"description\": \"The device model.\"\n            },\n            \"type\": {\n        \
  \      \"type\": \"string\",\n              \"description\": \"The device type.\"\n            }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/customer-io/refs/heads/main/json-schema/customer-io-event-schema.json
tags:
- Behavioral Data
- Broadcasts
- Campaigns
- CDP
- Customer Data
- Customer Data Platform
- Data Ingestion
- Email
- Event Tracking
- Marketing Automation
- Messaging
- Push Notifications
- Segments
- SMS
- Transactional Email
title: Customer.io Event
---
