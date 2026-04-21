---
description: Response containing catalog items and facets for a shop.
layout: schema
name: ShopResponse
properties_list:
- description: The unique identifier of the shop.
  name: shopID
  type: string
- description: List of catalog items.
  name: items
  type: array
- description: List of filter facets.
  name: facets
  type: array
provider_name: Ariba Guided Buying
provider_slug: ariba-guided-buying
schema_file: json-schema/catalog-shop-api-shop-response-schema.json
slug: catalog-shop-api-shop-response
tags:
- B2B
- Catalog
- ERP
- Procurement
- Requisitions
- SAP
- Supply Chain
title: ShopResponse
---
