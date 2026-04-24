---
description: An event in the Boltic Streams real-time event streaming system, representing a tracked action from a website, mobile app, or server.
layout: schema
name: Boltic Stream Event
properties_list:
- description: Unique identifier for the event
  name: id
  type: string
- description: ID of the stream source that received the event
  name: sourceId
  type: string
- description: Event type name (e.g., page_view, purchase, signup)
  name: type
  type: string
- description: Custom event properties
  name: properties
  type: object
- description: Contextual information about the event
  name: context
  type: object
- description: Identified user ID
  name: userId
  type: string
- description: Anonymous user identifier
  name: anonymousId
  type: string
- description: Client-side timestamp of when the event occurred
  name: timestamp
  type: string
- description: Server-side timestamp of when the event was received
  name: receivedAt
  type: string
provider_name: Boltic
provider_slug: boltic
schema_file: json-schema/boltic-stream-event.json
slug: boltic-stream-event
tags:
- Automation
- DataSync
- Gateways
- NoCode
- Streaming
- Workflows
title: Boltic Stream Event
---
