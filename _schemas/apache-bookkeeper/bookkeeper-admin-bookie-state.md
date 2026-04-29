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
source_filename: bookkeeper-admin-bookie-state-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-bookkeeper/refs/heads/main/json-schema/bookkeeper-admin-bookie-state-schema.json\",\n  \"title\": \"BookieState\",\n  \"description\": \"Current operational state of a BookKeeper bookie.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"running\": { \"type\": \"boolean\", \"description\": \"Whether the bookie is running.\", \"example\": true },\n    \"readOnly\": { \"type\": \"boolean\", \"description\": \"Whether the bookie is in read-only mode.\", \"example\": false },\n    \"shuttingDown\": { \"type\": \"boolean\", \"description\": \"Whether the bookie is shutting down.\", \"example\": false },\n    \"availableForHighPriorityWrites\": { \"type\": \"boolean\", \"description\": \"Whether the bookie accepts high-priority writes.\", \"example\": true }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-bookkeeper/refs/heads/main/json-schema/bookkeeper-admin-bookie-state-schema.json
tags:
- Apache
- Distributed Systems
- Log Storage
- Open Source
- Storage
- Streaming
title: BookieState
---
