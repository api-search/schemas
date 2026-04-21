---
description: A catalog item from a public catalog on SAP Business Network.
layout: schema
name: CatalogItem
properties_list:
- description: External product identifier.
  name: extProductId
  type: string
- description: Lead time in days.
  name: leadTime
  type: integer
- description: Manufacturer code.
  name: manufactCode
  type: string
- description: Manufacturer name.
  name: manufactName
  type: string
- description: Item price.
  name: price
  type: number
- description: Vendor identifier.
  name: vendor
  type: string
- description: Vendor display name.
  name: vendorName
  type: string
- description: Vendor-specific part identifier.
  name: vendorPartId
  type: string
provider_name: Ariba Guided Buying
provider_slug: ariba-guided-buying
schema_file: json-schema/catalog-shop-api-catalog-item-schema.json
slug: catalog-shop-api-catalog-item
tags:
- B2B
- Catalog
- ERP
- Procurement
- Requisitions
- SAP
- Supply Chain
title: CatalogItem
---
