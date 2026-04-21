---
description: ''
layout: schema
name: PickupRequest
properties_list:
- description: PRO number for the shipment
  name: proNumber
  type: string
- description: Requested pickup date
  name: pickupDate
  type: string
- description: Time freight will be ready (HH:MM)
  name: readyTime
  type: string
- description: Facility closing time (HH:MM)
  name: closeTime
  type: string
provider_name: ArcBest
provider_slug: arcbest
schema_file: json-schema/arcbest-api-pickup-request-schema.json
slug: arcbest-api-pickup-request
tags:
- Logistics
- Freight
- LTL
- Supply Chain
- Shipping
- Transportation
title: PickupRequest
---
