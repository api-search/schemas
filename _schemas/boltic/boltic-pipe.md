---
description: A Boltic Pipe is a data synchronization pipeline that connects a data source to a destination with configurable scheduling and field mappings.
layout: schema
name: Boltic Pipe
properties_list:
- description: Unique identifier for the pipe
  name: id
  type: string
- description: Human-readable name for the pipe
  name: name
  type: string
- description: Description of the data sync pipeline
  name: description
  type: string
- description: Current status of the pipe
  name: status
  type: string
- description: ''
  name: source
  type: object
- description: ''
  name: destination
  type: object
- description: ''
  name: schedule
  type: object
- description: Timestamp of the last successful sync
  name: lastSyncAt
  type: string
- description: Total rows synced since creation
  name: rowsSynced
  type: integer
- description: ''
  name: createdAt
  type: string
- description: ''
  name: updatedAt
  type: string
provider_name: Boltic
provider_slug: boltic
schema_file: json-schema/boltic-pipe.json
slug: boltic-pipe
tags:
- Automation
- DataSync
- Gateways
- NoCode
- Streaming
- Workflows
title: Boltic Pipe
---
