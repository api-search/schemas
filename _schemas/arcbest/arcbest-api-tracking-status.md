---
description: ''
layout: schema
name: TrackingStatus
properties_list:
- description: PRO number
  name: proNumber
  type: string
- description: Current shipment status
  name: status
  type: string
- description: Last known location
  name: lastLocation
  type: string
- description: Estimated delivery date
  name: estimatedDelivery
  type: string
- description: ''
  name: events
  type: array
provider_name: ArcBest
provider_slug: arcbest
schema_file: json-schema/arcbest-api-tracking-status-schema.json
slug: arcbest-api-tracking-status
tags:
- Logistics
- Freight
- LTL
- Supply Chain
- Shipping
- Transportation
title: TrackingStatus
---
