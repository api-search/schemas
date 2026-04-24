---
description: A Boltic Table is a no-code database entity for storing and managing structured data with a defined column schema.
layout: schema
name: Boltic Table
properties_list:
- description: Unique identifier for the table
  name: id
  type: string
- description: Human-readable name for the table
  name: name
  type: string
- description: Description of the table's purpose
  name: description
  type: string
- description: Schema definition of the table columns
  name: columns
  type: array
- description: Number of rows in the table
  name: rowCount
  type: integer
- description: ''
  name: createdAt
  type: string
- description: ''
  name: updatedAt
  type: string
provider_name: Boltic
provider_slug: boltic
schema_file: json-schema/boltic-table.json
slug: boltic-table
tags:
- Automation
- DataSync
- Gateways
- NoCode
- Streaming
- Workflows
title: Boltic Table
---
