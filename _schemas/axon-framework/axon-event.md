---
description: ''
layout: schema
name: Event
properties_list:
- description: ''
  name: messageIdentifier
  type: string
- description: ''
  name: aggregateIdentifier
  type: string
- description: ''
  name: aggregateSequenceNumber
  type: integer
- description: ''
  name: aggregateType
  type: string
- description: ''
  name: timestamp
  type: integer
- description: ''
  name: payloadType
  type: string
- description: ''
  name: payloadRevision
  type: string
- description: ''
  name: payloadData
  type: string
- description: ''
  name: metaData
  type: object
provider_name: Axon Framework
provider_slug: axon-framework
schema_file: json-schema/axon-event-schema.json
slug: axon-event
source_filename: axon-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Event\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"messageIdentifier\": {\n      \"type\": \"string\"\n    },\n    \"aggregateIdentifier\": {\n      \"type\": \"string\"\n    },\n    \"aggregateSequenceNumber\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"aggregateType\": {\n      \"type\": \"string\"\n    },\n    \"timestamp\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"payloadType\": {\n      \"type\": \"string\"\n    },\n    \"payloadRevision\": {\n      \"type\": \"string\"\n    },\n    \"payloadData\": {\n      \"type\": \"string\"\n    },\n    \"metaData\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/axon-framework/refs/heads/main/json-schema/axon-event-schema.json
tags:
- CQRS
- Event Sourcing
- Event-Driven
- Java
- Messaging
- Microservices
title: Event
---
