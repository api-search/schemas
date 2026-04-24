---
description: JSON Schema for a CargoSmart container tracking record including event history and vessel information.
layout: schema
name: CargoSmart Container Tracking
properties_list:
- description: ISO 6346 container number (e.g., MSCU1234567)
  name: containerId
  type: string
- description: ISO container type code
  name: containerType
  type: string
- description: Ocean carrier SCAC code
  name: carrierCode
  type: string
- description: ''
  name: vesselName
  type: string
- description: ''
  name: voyageNumber
  type: string
- description: ''
  name: currentStatus
  type: string
- description: ''
  name: originPort
  type: object
- description: ''
  name: destinationPort
  type: object
- description: Estimated arrival at destination port
  name: estimatedArrival
  type: string
- description: Actual arrival at destination port
  name: actualArrival
  type: string
- description: Chronological list of tracking events
  name: events
  type: array
- description: ''
  name: lastUpdated
  type: string
provider_name: CargoSmart
provider_slug: cargosmart
schema_file: json-schema/cargosmart-container-schema.json
slug: cargosmart-container
tags:
- Booking
- Container
- Documentation
- GSBN
- IQAX
- Logistics
- Maritime
- Ocean Freight
- Schedule
- Shipping
- Supply Chain
- Tracking
- Visibility
- Vessel
title: CargoSmart Container Tracking
---
