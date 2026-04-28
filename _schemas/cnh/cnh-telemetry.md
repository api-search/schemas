---
description: 'ISO 15143-3 vehicle telemetry payload returned by the CNH FieldOps API. Two profiles are supported: CP (CAN Parameter) and MH (Machine Health).'
layout: schema
name: CNH FieldOps Vehicle Telemetry
properties_list:
- description: ''
  name: vehicleId
  type: string
- description: CP = CAN Parameter profile (default). MH = Machine Health profile.
  name: profile
  type: string
- description: ''
  name: windowStart
  type: string
- description: ''
  name: windowEnd
  type: string
- description: ''
  name: location
  type: object
- description: Engine operating hours over the window.
  name: operatingHours
  type: number
- description: Engine idle hours over the window.
  name: idleHours
  type: number
- description: Fraction of tank fuel remaining at end of window.
  name: fuelRemainingRatio
  type: number
- description: Diesel Exhaust Fluid remaining (liters).
  name: defRemaining
  type: number
- description: Peak ground speed observed during the window (km/h).
  name: peakDailySpeed
  type: number
- description: Total distance travelled in the window (km).
  name: distance
  type: number
- description: Comma-separated error/quality tags (e.g. NO_GPS_FIX, NULL_DATA, UNREALISTIC_VALUE).
  name: errorTags
  type: string
- description: ''
  name: faultCodes
  type: array
provider_name: CNH
provider_slug: cnh
schema_file: json-schema/cnh-telemetry-schema.json
slug: cnh-telemetry
tags:
- Agriculture
- Construction
- Telematics
- Equipment
- FieldOps
title: CNH FieldOps Vehicle Telemetry
---
