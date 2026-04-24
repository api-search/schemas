---
description: JSON Schema for a Blue Yonder WMS inventory position representing stock at a warehouse location.
layout: schema
name: Blue Yonder Inventory Position
properties_list:
- description: Unique inventory position identifier
  name: positionId
  type: string
- description: Item/SKU identifier
  name: itemId
  type: string
- description: ''
  name: itemDescription
  type: string
- description: Warehouse location identifier (bin, rack, slot)
  name: locationId
  type: string
- description: ''
  name: locationName
  type: string
- description: Warehouse zone (e.g., Receiving, Storage, Shipping)
  name: zone
  type: string
- description: ''
  name: quantityOnHand
  type: number
- description: ''
  name: quantityAvailable
  type: number
- description: ''
  name: quantityReserved
  type: number
- description: Unit of measure (e.g., EA, CS, LB, KG)
  name: unitOfMeasure
  type: string
- description: ''
  name: lotNumber
  type: string
- description: ''
  name: serialNumber
  type: string
- description: ''
  name: expirationDate
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: lastUpdated
  type: string
provider_name: blue-yonder
provider_slug: blue-yonder
schema_file: json-schema/blue-yonder-inventory-schema.json
slug: blue-yonder-inventory
tags: []
title: Blue Yonder Inventory Position
---
