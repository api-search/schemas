---
description: Represents a telemetry event sent to Honeycomb via the Events API. Events are the fundamental unit of data in Honeycomb, containing structured key-value pairs that describe an operation or occurrence in your system.
layout: schema
name: Honeycomb Event
properties_list:
- description: The event's timestamp in ISO8601 or RFC3339 format. Defaults to the server's current time if not provided.
  name: time
  type: string
- description: An integer representing the sampling denominator. A value of 10 means one in ten events was kept during sampling.
  name: samplerate
  type: integer
- description: The event payload containing custom fields as key-value pairs. Fields become columns in the Honeycomb dataset.
  name: data
  type: object
provider_name: honeycomb
provider_slug: honeycomb
schema_file: json-schema/honeycomb-event-schema.json
slug: honeycomb-event
source_filename: honeycomb-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://honeycomb.io/schemas/honeycomb/event.json\",\n  \"title\": \"Honeycomb Event\",\n  \"description\": \"Represents a telemetry event sent to Honeycomb via the Events API. Events are the fundamental unit of data in Honeycomb, containing structured key-value pairs that describe an operation or occurrence in your system.\",\n  \"type\": \"object\",\n  \"required\": [\"data\"],\n  \"properties\": {\n    \"time\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The event's timestamp in ISO8601 or RFC3339 format. Defaults to the server's current time if not provided.\"\n    },\n    \"samplerate\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"description\": \"An integer representing the sampling denominator. A value of 10 means one in ten events was kept during sampling.\"\n    },\n    \"data\": {\n      \"type\": \"object\",\n     \
  \ \"description\": \"The event payload containing custom fields as key-value pairs. Fields become columns in the Honeycomb dataset.\",\n      \"additionalProperties\": true,\n      \"properties\": {\n        \"trace.trace_id\": {\n          \"type\": \"string\",\n          \"description\": \"The trace identifier linking related spans together.\"\n        },\n        \"trace.span_id\": {\n          \"type\": \"string\",\n          \"description\": \"The unique identifier for this span within a trace.\"\n        },\n        \"trace.parent_id\": {\n          \"type\": \"string\",\n          \"description\": \"The span ID of the parent span in a trace.\"\n        },\n        \"service_name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the service that generated this event.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the operation or event.\"\n        },\n        \"duration_ms\": {\n        \
  \  \"type\": \"number\",\n          \"minimum\": 0,\n          \"description\": \"The duration of the operation in milliseconds.\"\n        },\n        \"error\": {\n          \"type\": [\"string\", \"boolean\"],\n          \"description\": \"Indicates whether the operation resulted in an error.\"\n        },\n        \"http.method\": {\n          \"type\": \"string\",\n          \"description\": \"The HTTP method of the request.\",\n          \"enum\": [\"GET\", \"POST\", \"PUT\", \"PATCH\", \"DELETE\", \"HEAD\", \"OPTIONS\"]\n        },\n        \"http.status_code\": {\n          \"type\": \"integer\",\n          \"minimum\": 100,\n          \"maximum\": 599,\n          \"description\": \"The HTTP response status code.\"\n        },\n        \"http.route\": {\n          \"type\": \"string\",\n          \"description\": \"The matched route pattern for the HTTP request.\"\n        },\n        \"http.url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"\
  description\": \"The full URL of the HTTP request.\"\n        }\n      }\n    }\n  },\n  \"$defs\": {\n    \"BatchEventResponse\": {\n      \"type\": \"object\",\n      \"description\": \"Response for an individual event within a batch submission.\",\n      \"properties\": {\n        \"status\": {\n          \"type\": \"integer\",\n          \"description\": \"The HTTP status code for this individual event. 202 indicates successful queuing.\"\n        },\n        \"error\": {\n          \"type\": \"string\",\n          \"description\": \"An error message if the event failed processing.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/honeycomb/refs/heads/main/json-schema/honeycomb-event-schema.json
tags: []
title: Honeycomb Event
---
