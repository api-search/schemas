---
description: A detailed order with campaigns and datasets.
layout: schema
name: Order
properties_list:
- description: Order identifier.
  name: orderId
  type: string
- description: Order status.
  name: status
  type: string
- description: Order creation timestamp.
  name: createdAt
  type: string
- description: ''
  name: campaigns
  type: array
provider_name: Arlula
provider_slug: arlula
schema_file: json-schema/arlula-order-schema.json
slug: arlula-order
tags:
- Earth Observation
- Geospatial
- Imagery
- Remote Sensing
- Satellites
title: Order
---
