---
description: A route in the Boltic Gateway that defines how incoming API requests are matched and forwarded to backend services.
layout: schema
name: Boltic Gateway Route
properties_list:
- description: Unique identifier for the route
  name: id
  type: string
- description: Human-readable name for the route
  name: name
  type: string
- description: HTTP methods this route responds to
  name: methods
  type: array
- description: URL paths that match this route
  name: paths
  type: array
- description: ID of the backend service to route to
  name: serviceId
  type: string
- description: Whether to strip the matched path prefix before forwarding
  name: stripPath
  type: boolean
- description: Whether to preserve the original Host header
  name: preserveHost
  type: boolean
- description: ''
  name: protocols
  type: array
- description: List of plugin IDs applied to this route
  name: plugins
  type: array
- description: ''
  name: status
  type: string
- description: ''
  name: createdAt
  type: string
- description: ''
  name: updatedAt
  type: string
provider_name: Boltic
provider_slug: boltic
schema_file: json-schema/boltic-route.json
slug: boltic-route
tags:
- Automation
- DataSync
- Gateways
- NoCode
- Streaming
- Workflows
title: Boltic Gateway Route
---
