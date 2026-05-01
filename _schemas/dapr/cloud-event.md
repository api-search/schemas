---
description: A CloudEvents 1.0 specification envelope used by Dapr for pub/sub messaging. All published events are wrapped in this format unless raw payload mode is enabled.
layout: schema
name: Dapr CloudEvent
properties_list:
- description: The version of the CloudEvents specification.
  name: specversion
  type: string
- description: The type of the event.
  name: type
  type: string
- description: The source of the event, typically the app ID of the publisher.
  name: source
  type: string
- description: Unique identifier for the event.
  name: id
  type: string
- description: The subject of the event in context of the event producer.
  name: subject
  type: string
- description: Timestamp of when the event occurred (RFC 3339).
  name: time
  type: string
- description: Content type of the data attribute (e.g., application/json).
  name: datacontenttype
  type: string
- description: The event payload data.
  name: data
  type: object
- description: The topic the event was published to (Dapr extension).
  name: topic
  type: string
- description: The name of the pub/sub component (Dapr extension).
  name: pubsubname
  type: string
- description: The distributed tracing identifier (Dapr extension).
  name: traceid
  type: string
- description: The W3C trace context traceparent header value (Dapr extension).
  name: traceparent
  type: string
- description: The W3C trace context tracestate header value (Dapr extension).
  name: tracestate
  type: string
provider_name: Dapr
provider_slug: dapr
schema_file: json-schema/cloud-event.json
slug: cloud-event
source_filename: cloud-event.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/dapr/blob/main/json-schema/cloud-event.json\",\n  \"title\": \"Dapr CloudEvent\",\n  \"description\": \"A CloudEvents 1.0 specification envelope used by Dapr for pub/sub messaging. All published events are wrapped in this format unless raw payload mode is enabled.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"specversion\",\n    \"type\",\n    \"source\",\n    \"id\"\n  ],\n  \"properties\": {\n    \"specversion\": {\n      \"type\": \"string\",\n      \"description\": \"The version of the CloudEvents specification.\",\n      \"enum\": [\n        \"1.0\"\n      ]\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the event.\"\n    },\n    \"source\": {\n      \"type\": \"string\",\n      \"description\": \"The source of the event, typically the app ID of the publisher.\"\n    },\n    \"id\": {\n      \"type\": \"\
  string\",\n      \"description\": \"Unique identifier for the event.\"\n    },\n    \"subject\": {\n      \"type\": \"string\",\n      \"description\": \"The subject of the event in context of the event producer.\"\n    },\n    \"time\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of when the event occurred (RFC 3339).\"\n    },\n    \"datacontenttype\": {\n      \"type\": \"string\",\n      \"description\": \"Content type of the data attribute (e.g., application/json).\"\n    },\n    \"data\": {\n      \"description\": \"The event payload data.\"\n    },\n    \"topic\": {\n      \"type\": \"string\",\n      \"description\": \"The topic the event was published to (Dapr extension).\"\n    },\n    \"pubsubname\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the pub/sub component (Dapr extension).\"\n    },\n    \"traceid\": {\n      \"type\": \"string\",\n      \"description\": \"The distributed tracing identifier\
  \ (Dapr extension).\"\n    },\n    \"traceparent\": {\n      \"type\": \"string\",\n      \"description\": \"The W3C trace context traceparent header value (Dapr extension).\"\n    },\n    \"tracestate\": {\n      \"type\": \"string\",\n      \"description\": \"The W3C trace context tracestate header value (Dapr extension).\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dapr/refs/heads/main/json-schema/cloud-event.json
tags:
- Distributed Systems
- Microservices
- Platform
- Pub/Sub
- State Management
- Workflows
title: Dapr CloudEvent
---
