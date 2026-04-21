---
description: Request body for ordering a future satellite capture.
layout: schema
name: TaskingOrderRequest
properties_list:
- description: Ordering ID of the tasking opportunity.
  name: id
  type: string
- description: Bundle key for this order.
  name: bundleKey
  type: string
- description: EULA identifier.
  name: eula
  type: string
- description: Maximum acceptable cloud cover percentage.
  name: cloud
  type: integer
- description: Priority level for the capture.
  name: priorityKey
  type: string
- description: ''
  name: emails
  type: array
- description: ''
  name: webhooks
  type: array
- description: Optional coupon code.
  name: coupon
  type: string
provider_name: Arlula
provider_slug: arlula
schema_file: json-schema/arlula-tasking-order-request-schema.json
slug: arlula-tasking-order-request
tags:
- Earth Observation
- Geospatial
- Imagery
- Remote Sensing
- Satellites
title: TaskingOrderRequest
---
