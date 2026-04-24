---
description: A Best Buy store location with operational details.
layout: schema
name: Store
properties_list:
- description: Unique store identifier.
  name: storeId
  type: integer
- description: Short store name.
  name: name
  type: string
- description: Full store name including address.
  name: longName
  type: string
- description: Street address of the store.
  name: address
  type: string
- description: Secondary address line (suite, building, etc.).
  name: address2
  type: string
- description: City where the store is located.
  name: city
  type: string
- description: Two-letter US state abbreviation.
  name: state
  type: string
- description: US postal code.
  name: zipcode
  type: string
- description: Store phone number.
  name: phone
  type: string
- description: Store latitude coordinate.
  name: lat
  type: number
- description: Store longitude coordinate.
  name: lng
  type: number
- description: Distance from the search location in miles (when area query is used).
  name: distance
  type: number
- description: Store format type.
  name: storeType
  type: string
- description: Store hours summary.
  name: hours
  type: string
- description: GMT offset for the store's timezone.
  name: gmtOffset
  type: integer
- description: Services offered at this store location.
  name: services
  type: array
provider_name: Best Buy
provider_slug: best-buy
schema_file: json-schema/stores-api-store-schema.json
slug: stores-api-store
tags:
- Retail
- Consumer Electronics
- E-Commerce
- Products
- Stores
title: Store
---
