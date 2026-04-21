---
description: Subscription schema from ARGUS Enterprise API
layout: schema
name: Subscription
properties_list:
- description: Unique subscription identifier
  name: id
  type: string
- description: HTTPS endpoint URL for webhook delivery
  name: url
  type: string
- description: Event types this subscription receives
  name: eventTypes
  type: array
- description: Current subscription status
  name: status
  type: string
- description: Shared secret for HMAC-SHA256 signature verification of webhook payloads (only returned on creation)
  name: secret
  type: string
- description: Human-readable description of the subscription
  name: description
  type: string
- description: ''
  name: retryPolicy
  type: object
- description: ''
  name: createdAt
  type: string
- description: ''
  name: updatedAt
  type: string
provider_name: ARGUS Enterprise
provider_slug: argus-enterprise
schema_file: json-schema/argus-enterprise-subscription-schema.json
slug: argus-enterprise-subscription
tags:
- Altus Group
- Asset Management
- Cash Flow Modeling
- Commercial Real Estate
- Portfolio Management
- Valuation
title: Subscription
---
