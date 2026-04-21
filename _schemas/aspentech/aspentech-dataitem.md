---
description: JSON Schema for an AspenTech Inmation process data item (tag) including current value, quality, and historical data.
layout: schema
name: AspenTech Inmation Data Item
properties_list:
- description: Full hierarchical path to the data item in the Inmation system tree (e.g., /System/Core/Plant1/Temperature)
  name: path
  type: string
- description: Current process value - can be numeric, string, or boolean
  name: value
  type: object
- description: OPC UA/DA quality code (192=Good, 0=Bad, 64=Uncertain)
  name: quality
  type: integer
- description: Timestamp of the current value (ISO 8601 UTC)
  name: timestamp
  type: string
- description: Engineering unit for the value (e.g., degC, bar, m3/h)
  name: engineeringUnit
  type: string
- description: Type of Inmation item
  name: itemType
  type: string
- description: Item display name
  name: name
  type: string
- description: Item description
  name: description
  type: string
- description: High engineering range limit
  name: highLimit
  type: number
- description: Low engineering range limit
  name: lowLimit
  type: number
- description: High alarm threshold
  name: alarmHigh
  type: number
- description: Low alarm threshold
  name: alarmLow
  type: number
- description: Deadband for value change detection
  name: deadband
  type: number
provider_name: AspenTech
provider_slug: aspentech
schema_file: json-schema/aspentech-dataitem-schema.json
slug: aspentech-dataitem
tags:
- Industrial IoT
- Process Optimization
- Manufacturing
- Energy
- Chemicals
- Time Series
title: AspenTech Inmation Data Item
---
