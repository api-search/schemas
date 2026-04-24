---
description: A Best Buy product with pricing, availability, and metadata.
layout: schema
name: Product
properties_list:
- description: Unique Best Buy product identifier (SKU number).
  name: sku
  type: integer
- description: Product display name.
  name: name
  type: string
- description: Regular (non-sale) price in USD.
  name: regularPrice
  type: number
- description: Current sale price in USD.
  name: salePrice
  type: number
- description: Whether the product is currently on sale.
  name: onSale
  type: boolean
- description: Product manufacturer or brand name.
  name: manufacturer
  type: string
- description: Manufacturer model number.
  name: modelNumber
  type: string
- description: Brief product description.
  name: shortDescription
  type: string
- description: Detailed product description.
  name: longDescription
  type: string
- description: URL of the primary product image.
  name: image
  type: string
- description: URL of the product page on bestbuy.com.
  name: url
  type: string
- description: URL for adding this product to the shopping cart.
  name: addToCartUrl
  type: string
- description: Whether the product is available for in-store purchase.
  name: inStoreAvailability
  type: boolean
- description: Whether the product is available online.
  name: onlineAvailability
  type: boolean
- description: Product type (HardGood, Movie, Music, Game, Software, etc.).
  name: type
  type: string
- description: Product class name.
  name: class
  type: string
- description: Product class identifier.
  name: classId
  type: integer
- description: Product subclass name.
  name: subclass
  type: string
- description: Product subclass identifier.
  name: subclassId
  type: integer
- description: Department name.
  name: department
  type: string
- description: Department identifier.
  name: departmentId
  type: integer
- description: Hierarchical category path from root to this product's category.
  name: categoryPath
  type: array
- description: Total number of customer reviews.
  name: customerReviewCount
  type: integer
- description: Average customer review rating out of 5.
  name: customerReviewAverage
  type: number
- description: Date and time the price was last updated.
  name: priceUpdateDate
  type: string
provider_name: Best Buy
provider_slug: best-buy
schema_file: json-schema/products-api-product-schema.json
slug: products-api-product
tags:
- Retail
- Consumer Electronics
- E-Commerce
- Products
- Stores
title: Product
---
