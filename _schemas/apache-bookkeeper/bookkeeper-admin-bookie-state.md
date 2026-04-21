---
description: Current operational state of a BookKeeper bookie.
layout: schema
name: BookieState
properties_list:
- description: Whether the bookie is running.
  name: running
  type: boolean
- description: Whether the bookie is in read-only mode.
  name: readOnly
  type: boolean
- description: Whether the bookie is shutting down.
  name: shuttingDown
  type: boolean
- description: Whether the bookie accepts high-priority writes.
  name: availableForHighPriorityWrites
  type: boolean
provider_name: Apache BookKeeper
provider_slug: apache-bookkeeper
schema_file: json-schema/bookkeeper-admin-bookie-state-schema.json
slug: bookkeeper-admin-bookie-state
tags:
- Apache
- Distributed Systems
- Log Storage
- Open Source
- Storage
- Streaming
title: BookieState
---
