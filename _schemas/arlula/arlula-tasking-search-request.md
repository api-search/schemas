---
description: Request body for searching future satellite capture opportunities.
layout: schema
name: TaskingSearchRequest
properties_list:
- description: Start of the search window.
  name: start
  type: string
- description: End of the search window.
  name: end
  type: string
- description: Maximum ground sample distance in meters.
  name: gsd
  type: number
- description: Latitude of the area of interest.
  name: lat
  type: number
- description: Longitude of the area of interest.
  name: long
  type: number
- description: Maximum acceptable cloud cover percentage.
  name: cloud
  type: integer
- description: Maximum off-nadir angle in degrees.
  name: offNadir
  type: number
- description: ''
  name: suppliers
  type: array
- description: ''
  name: platformTypes
  type: array
- description: ''
  name: sensorTypes
  type: array
provider_name: Arlula
provider_slug: arlula
schema_file: json-schema/arlula-tasking-search-request-schema.json
slug: arlula-tasking-search-request
tags:
- Earth Observation
- Geospatial
- Imagery
- Remote Sensing
- Satellites
title: TaskingSearchRequest
---
