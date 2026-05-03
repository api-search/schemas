---
description: Schema for a domain event in an event-sourced or event-driven system following CloudEvents conventions.
layout: schema
name: Domain Event
properties_list:
- description: CloudEvents specification version.
  name: specversion
  type: string
- description: Event type in reverse DNS notation.
  name: type
  type: string
- description: Identifies the event producer (bounded context or service).
  name: source
  type: string
- description: Unique identifier for this event occurrence (UUID recommended).
  name: id
  type: string
- description: Timestamp when the event occurred (RFC 3339).
  name: time
  type: string
- description: Subject/entity identifier this event relates to (e.g., order ID).
  name: subject
  type: string
- description: Content type of the data field.
  name: datacontenttype
  type: string
- description: URI of the schema the data attribute conforms to.
  name: dataschema
  type: string
- description: Event payload. Schema depends on event type.
  name: data
  type: object
- description: Correlation ID for tracing requests across service boundaries.
  name: correlationId
  type: string
- description: ID of the command or event that caused this event.
  name: causationId
  type: string
- description: Identifier of the domain aggregate this event belongs to.
  name: aggregateId
  type: string
- description: Type of the domain aggregate (e.g., Order, Customer, Payment).
  name: aggregateType
  type: string
- description: Optimistic concurrency version of the aggregate after this event.
  name: aggregateVersion
  type: integer
- description: Additional metadata (user ID, tenant ID, trace context, etc.).
  name: metadata
  type: object
provider_name: Scalable Software and Systems
provider_slug: scalable-software-and-systems
schema_file: json-schema/scalable-software-and-systems-event-schema.json
slug: scalable-software-and-systems-event
source_filename: scalable-software-and-systems-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://api-evangelist.com/schemas/scalable-software-and-systems/domain-event\",\n  \"title\": \"Domain Event\",\n  \"description\": \"Schema for a domain event in an event-sourced or event-driven system following CloudEvents conventions.\",\n  \"type\": \"object\",\n  \"required\": [\"specversion\", \"type\", \"source\", \"id\", \"time\"],\n  \"properties\": {\n    \"specversion\": {\n      \"type\": \"string\",\n      \"description\": \"CloudEvents specification version.\",\n      \"enum\": [\"1.0\"],\n      \"example\": \"1.0\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Event type in reverse DNS notation.\",\n      \"example\": \"com.example.order.placed\"\n    },\n    \"source\": {\n      \"type\": \"string\",\n      \"format\": \"uri-reference\",\n      \"description\": \"Identifies the event producer (bounded context or service).\",\n      \"example\": \"\
  /orders-service\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for this event occurrence (UUID recommended).\",\n      \"example\": \"b2c3d4e5-f6a7-8901-bcde-f01234567890\"\n    },\n    \"time\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the event occurred (RFC 3339).\"\n    },\n    \"subject\": {\n      \"type\": \"string\",\n      \"description\": \"Subject/entity identifier this event relates to (e.g., order ID).\",\n      \"example\": \"order-12345\"\n    },\n    \"datacontenttype\": {\n      \"type\": \"string\",\n      \"description\": \"Content type of the data field.\",\n      \"default\": \"application/json\",\n      \"example\": \"application/json\"\n    },\n    \"dataschema\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URI of the schema the data attribute conforms to.\"\n    },\n    \"data\": {\n      \"type\": \"object\"\
  ,\n      \"description\": \"Event payload. Schema depends on event type.\",\n      \"additionalProperties\": true\n    },\n    \"correlationId\": {\n      \"type\": \"string\",\n      \"description\": \"Correlation ID for tracing requests across service boundaries.\"\n    },\n    \"causationId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the command or event that caused this event.\"\n    },\n    \"aggregateId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the domain aggregate this event belongs to.\"\n    },\n    \"aggregateType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of the domain aggregate (e.g., Order, Customer, Payment).\"\n    },\n    \"aggregateVersion\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"Optimistic concurrency version of the aggregate after this event.\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"description\": \"Additional metadata (user\
  \ ID, tenant ID, trace context, etc.).\",\n      \"properties\": {\n        \"userId\": { \"type\": \"string\" },\n        \"tenantId\": { \"type\": \"string\" },\n        \"traceId\": { \"type\": \"string\" },\n        \"spanId\": { \"type\": \"string\" }\n      },\n      \"additionalProperties\": true\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/scalable-software-and-systems/refs/heads/main/json-schema/scalable-software-and-systems-event-schema.json
tags:
- API First
- Architecture Patterns
- CQRS
- Distributed Systems
- Enterprise
- Event Driven
- Microservices
- Scalable Architecture
- Software Engineering
- Systems Design
title: Domain Event
---
