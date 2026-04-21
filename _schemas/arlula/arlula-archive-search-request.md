---
description: Request body for searching the archive imagery catalog.
layout: schema
name: ArchiveSearchRequest
properties_list:
- description: Start date for imagery search (YYYY-MM-DD).
  name: start
  type: string
- description: End date for imagery search (YYYY-MM-DD).
  name: end
  type: string
- description: Maximum ground sample distance in meters.
  name: gsd
  type: number
- description: Latitude of the point of interest.
  name: lat
  type: number
- description: Longitude of the point of interest.
  name: long
  type: number
- description: Maximum cloud cover percentage (0-100).
  name: cloud
  type: integer
- description: Maximum off-nadir angle in degrees.
  name: offNadir
  type: number
- description: ''
  name: suppliers
  type: array
provider_name: Arlula
provider_slug: arlula
schema_file: json-schema/arlula-archive-search-request-schema.json
slug: arlula-archive-search-request
tags:
- Earth Observation
- Geospatial
- Imagery
- Remote Sensing
- Satellites
title: ArchiveSearchRequest
---
