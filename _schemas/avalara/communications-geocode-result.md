---
description: GeocodeResult schema from Avalara API
layout: schema
name: GeocodeResult
properties_list:
- description: ''
  name: ref
  type: string
- description: ''
  name: cass
  type: object
- description: Census block group
  name: cBlk
  type: string
- description: Census tract
  name: cTrc
  type: string
- description: Error message if geocoding failed
  name: err
  type: string
- description: Whether geocoding was successful
  name: geo
  type: boolean
- description: ''
  name: lat
  type: number
- description: ''
  name: long
  type: number
- description: PCode for the determined jurisdiction
  name: pcd
  type: integer
- description: FIPS code
  name: fips
  type: string
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/communications-geocode-result-schema.json
slug: communications-geocode-result
tags:
- Taxes
title: GeocodeResult
---
