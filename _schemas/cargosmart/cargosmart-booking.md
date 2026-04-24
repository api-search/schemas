---
description: JSON Schema for a CargoSmart ocean container booking request/confirmation.
layout: schema
name: CargoSmart Container Booking
properties_list:
- description: ''
  name: bookingId
  type: string
- description: Carrier-assigned booking confirmation number
  name: bookingNumber
  type: string
- description: Ocean carrier SCAC code (e.g., MSCU, HLCU, CMDU)
  name: carrierCode
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: originPort
  type: object
- description: ''
  name: destinationPort
  type: object
- description: ''
  name: requestedDepartureDate
  type: string
- description: ''
  name: confirmedVessel
  type: string
- description: ''
  name: confirmedVoyage
  type: string
- description: ''
  name: containers
  type: array
- description: ''
  name: cargoDescription
  type: string
- description: ''
  name: shipper
  type: object
- description: ''
  name: consignee
  type: object
- description: ''
  name: createdAt
  type: string
provider_name: CargoSmart
provider_slug: cargosmart
schema_file: json-schema/cargosmart-booking-schema.json
slug: cargosmart-booking
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
title: CargoSmart Container Booking
---
