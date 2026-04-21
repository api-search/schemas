---
description: Event schema from ARGUS Enterprise API
layout: schema
name: Event
properties_list:
- description: Unique event identifier
  name: id
  type: string
- description: Subscription that received this event
  name: subscriptionId
  type: string
- description: Type of event
  name: eventType
  type: string
- description: Delivery status
  name: status
  type: string
- description: Event payload data
  name: payload
  type: object
- description: ''
  name: deliveryAttempts
  type: array
- description: ''
  name: createdAt
  type: string
provider_name: ARGUS Enterprise
provider_slug: argus-enterprise
schema_file: json-schema/argus-enterprise-event-schema.json
slug: argus-enterprise-event
tags:
- Altus Group
- Asset Management
- Cash Flow Modeling
- Commercial Real Estate
- Portfolio Management
- Valuation
title: Event
---
