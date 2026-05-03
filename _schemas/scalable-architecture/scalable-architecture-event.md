---
description: Describes a domain event in an event-driven scalable architecture, following CloudEvents conventions. Domain events enable loose coupling between microservices through async message passing over Kafka, RabbitMQ, or cloud message brokers.
layout: schema
name: Domain Event
properties_list:
- description: CloudEvents specification version.
  name: specversion
  type: string
- description: Unique identifier for this event occurrence.
  name: id
  type: string
- description: URI identifying the context in which the event occurred (typically the originating service).
  name: source
  type: string
- description: Event type in reverse-DNS notation describing the kind of occurrence.
  name: type
  type: string
- description: Identifies the subject of the event in the context of the source (e.g., entity ID).
  name: subject
  type: string
- description: Content type of the event data.
  name: datacontenttype
  type: string
- description: URI identifying the schema for the event data payload.
  name: dataschema
  type: string
- description: Timestamp of when the event occurred in RFC3339 format.
  name: time
  type: string
- description: Domain event payload specific to the event type.
  name: data
  type: object
- description: Key used to route the event to a specific Kafka partition for ordering guarantees.
  name: partitionkey
  type: string
- description: Correlation ID for tracing a business transaction across multiple services.
  name: correlationid
  type: string
- description: ID of the command or event that caused this event (event sourcing lineage).
  name: causationid
  type: string
- description: Additional metadata properties for routing, filtering, and tracing.
  name: metadata
  type: object
provider_name: Scalable Architecture
provider_slug: scalable-architecture
schema_file: json-schema/scalable-architecture-event-schema.json
slug: scalable-architecture-event
source_filename: scalable-architecture-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/scalable-architecture/main/json-schema/scalable-architecture-event-schema.json\",\n  \"title\": \"Domain Event\",\n  \"description\": \"Describes a domain event in an event-driven scalable architecture, following CloudEvents conventions. Domain events enable loose coupling between microservices through async message passing over Kafka, RabbitMQ, or cloud message brokers.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"source\", \"specversion\", \"type\"],\n  \"properties\": {\n    \"specversion\": {\n      \"type\": \"string\",\n      \"description\": \"CloudEvents specification version.\",\n      \"const\": \"1.0\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for this event occurrence.\",\n      \"format\": \"uuid\",\n      \"example\": \"96fb5f0b-001e-0108-6d02-a85e0000000\"\n    },\n\
  \    \"source\": {\n      \"type\": \"string\",\n      \"description\": \"URI identifying the context in which the event occurred (typically the originating service).\",\n      \"format\": \"uri\",\n      \"example\": \"/orders/service\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Event type in reverse-DNS notation describing the kind of occurrence.\",\n      \"pattern\": \"^[a-z][a-z0-9.]+$\",\n      \"examples\": [\n        \"com.example.orders.created\",\n        \"com.example.payments.completed\",\n        \"com.example.inventory.updated\"\n      ]\n    },\n    \"subject\": {\n      \"type\": \"string\",\n      \"description\": \"Identifies the subject of the event in the context of the source (e.g., entity ID).\",\n      \"example\": \"order-12345\"\n    },\n    \"datacontenttype\": {\n      \"type\": \"string\",\n      \"description\": \"Content type of the event data.\",\n      \"default\": \"application/json\",\n      \"examples\": [\"application/json\"\
  , \"application/avro\"]\n    },\n    \"dataschema\": {\n      \"type\": \"string\",\n      \"description\": \"URI identifying the schema for the event data payload.\",\n      \"format\": \"uri\"\n    },\n    \"time\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp of when the event occurred in RFC3339 format.\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-05-02T14:30:00Z\"\n    },\n    \"data\": {\n      \"type\": \"object\",\n      \"description\": \"Domain event payload specific to the event type.\",\n      \"additionalProperties\": true\n    },\n    \"partitionkey\": {\n      \"type\": \"string\",\n      \"description\": \"Key used to route the event to a specific Kafka partition for ordering guarantees.\",\n      \"example\": \"customer-456\"\n    },\n    \"correlationid\": {\n      \"type\": \"string\",\n      \"description\": \"Correlation ID for tracing a business transaction across multiple services.\",\n      \"format\": \"uuid\"\n    },\n\
  \    \"causationid\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the command or event that caused this event (event sourcing lineage).\",\n      \"format\": \"uuid\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"description\": \"Additional metadata properties for routing, filtering, and tracing.\",\n      \"properties\": {\n        \"retryCount\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of times this event has been retried.\",\n          \"minimum\": 0,\n          \"default\": 0\n        },\n        \"deadLetterQueue\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether this event has been moved to the dead letter queue.\",\n          \"default\": false\n        },\n        \"version\": {\n          \"type\": \"integer\",\n          \"description\": \"Schema version for event evolution.\",\n          \"minimum\": 1,\n          \"default\": 1\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/scalable-architecture/refs/heads/main/json-schema/scalable-architecture-event-schema.json
tags:
- Cloud Architecture
- Cloud Native
- Distributed Systems
- High Availability
- Infrastructure
- Microservices
- Performance
- Resilience
- Scalability
- Service Mesh
title: Domain Event
---
