---
description: AddressInfo schema from Avalara API
layout: schema
name: AddressInfo
properties_list:
- description: Street address line 1
  name: line1
  type: string
- description: Street address line 2
  name: line2
  type: string
- description: Street address line 3
  name: line3
  type: string
- description: City name
  name: city
  type: string
- description: State, province, or region code
  name: region
  type: string
- description: Postal code or ZIP code
  name: postalCode
  type: string
- description: Two-character ISO 3166 country code
  name: country
  type: string
- description: ''
  name: latitude
  type: number
- description: ''
  name: longitude
  type: number
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/avatax-rest-address-info-schema.json
slug: avatax-rest-address-info
tags:
- Taxes
title: AddressInfo
---
