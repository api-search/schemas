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
tags:
- CQRS
- Event Sourcing
- Event-Driven
- Java
- Messaging
- Microservices
title: Event
---
