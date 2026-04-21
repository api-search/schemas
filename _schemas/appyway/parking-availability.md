---
description: Real-time parking availability data from AppyWay
layout: schema
name: ParkingAvailability
properties_list:
- description: Unique parking location identifier
  name: locationId
  type: string
- description: Parking location name
  name: name
  type: string
- description: Number of available parking spaces
  name: availableSpaces
  type: integer
- description: Total number of parking spaces
  name: totalSpaces
  type: integer
- description: Current occupancy percentage
  name: occupancyPercent
  type: number
- description: Timestamp of availability data
  name: timestamp
  type: string
- description: Geographic coordinates of the parking location
  name: coordinates
  type: object
- description: Whether EV charging is available
  name: evCharging
  type: boolean
- description: Parking restrictions (residents only, time-limited, etc.)
  name: restrictions
  type: array
provider_name: AppyWay
provider_slug: appyway
schema_file: json-schema/parking-availability-schema.json
slug: parking-availability
tags:
- Parking
- Traffic
- Urban Mobility
- Smart Cities
- EV Charging
title: ParkingAvailability
---
