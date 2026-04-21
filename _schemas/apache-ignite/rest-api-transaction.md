---
description: Rest representation of transaction.
layout: schema
name: Transaction
properties_list:
- description: Transaction ID.
  name: id
  type: string
- description: Coordinator node.
  name: node
  type: string
- description: State.
  name: state
  type: string
- description: Type.
  name: type
  type: string
- description: Priority.
  name: priority
  type: string
- description: Start time.
  name: startTime
  type: string
provider_name: Apache Ignite
provider_slug: apache-ignite
schema_file: json-schema/rest-api-transaction-schema.json
slug: rest-api-transaction
tags:
- Caching
- Compute Grid
- Distributed Database
- In-Memory
- Open Source
- SQL
title: Transaction
---
