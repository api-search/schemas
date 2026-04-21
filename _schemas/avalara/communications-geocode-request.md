---
description: GeocodeRequest schema from Avalara API
layout: schema
name: GeocodeRequest
properties_list:
- description: Reference ID
  name: ref
  type: string
- description: Whether to return CASS-certified address
  name: cass
  type: boolean
- description: Street address
  name: addr
  type: string
- description: ''
  name: city
  type: string
- description: State abbreviation
  name: st
  type: string
- description: ZIP code
  name: zip
  type: string
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/communications-geocode-request-schema.json
slug: communications-geocode-request
tags:
- Taxes
title: GeocodeRequest
---
