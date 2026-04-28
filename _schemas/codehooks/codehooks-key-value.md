---
description: A key-value entry in the Codehooks key-value store, supporting string or object values with optional TTL-based expiration.
layout: schema
name: Codehooks Key-Value Entry
properties_list:
- description: The unique key identifier for the stored value.
  name: key
  type: string
- description: The stored value, which can be a string, number, or JSON object.
  name: value
  type: object
- description: Time-to-live in milliseconds for automatic expiration of the key-value pair.
  name: ttl
  type: integer
provider_name: Codehooks
provider_slug: codehooks
schema_file: json-schema/codehooks-key-value-schema.json
slug: codehooks-key-value
tags:
- Backend
- Database
- Events
- Hooks
- JavaScript
- NoSQL
- Queues
- Serverless
- Webhooks
- Workers
- Workflows
title: Codehooks Key-Value Entry
---
