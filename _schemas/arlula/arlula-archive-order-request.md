---
description: Request body for ordering archive imagery.
layout: schema
name: ArchiveOrderRequest
properties_list:
- description: Ordering ID of the archive scene to purchase.
  name: id
  type: string
- description: Bundle key selected from search results.
  name: bundleKey
  type: string
- description: EULA identifier accepted for this order.
  name: eula
  type: string
- description: ''
  name: emails
  type: array
- description: ''
  name: webhooks
  type: array
- description: Optional coupon code for discounts.
  name: coupon
  type: string
provider_name: Arlula
provider_slug: arlula
schema_file: json-schema/arlula-archive-order-request-schema.json
slug: arlula-archive-order-request
tags:
- Earth Observation
- Geospatial
- Imagery
- Remote Sensing
- Satellites
title: ArchiveOrderRequest
---
