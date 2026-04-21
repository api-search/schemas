---
description: The wrapper object for catalog entries of a given object type.
layout: schema
name: CatalogObject
properties_list:
- description: The type of this object.
  name: type
  type: string
- description: Unique ID for this CatalogObject.
  name: id
  type: string
- description: The version of the object for optimistic concurrency control.
  name: version
  type: integer
- description: Structured data for a CatalogItem.
  name: item_data
  type: object
provider_name: Block
provider_slug: block
schema_file: json-schema/block-catalog-object-schema.json
slug: block-catalog-object
tags:
- Commerce
- Cryptocurrency
- eCommerce
- Fintech
- Payments
- Point Of Sale
- Square
title: CatalogObject
---
