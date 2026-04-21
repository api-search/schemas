---
description: Location schema from Avalara API
layout: schema
name: Location
properties_list:
- description: PCode for jurisdiction
  name: pcd
  type: integer
- description: Country ISO code
  name: ctry
  type: string
- description: State abbreviation
  name: st
  type: string
- description: County name
  name: cty
  type: string
- description: ZIP code
  name: zip
  type: string
- description: Whether to geocode the address
  name: geo
  type: boolean
- description: Street address for geocoding
  name: addr
  type: string
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/communications-location-schema.json
slug: communications-location
tags:
- Taxes
title: Location
---
