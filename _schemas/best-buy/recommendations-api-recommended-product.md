---
description: A recommended product with essential display attributes.
layout: schema
name: RecommendedProduct
properties_list:
- description: Product SKU number.
  name: sku
  type: integer
- description: Product name variations.
  name: names
  type: object
- description: Product image URLs.
  name: images
  type: object
- description: Product pricing information.
  name: prices
  type: object
- description: Related URLs for the product.
  name: links
  type: object
- description: Rank position in the recommendation list.
  name: rank
  type: integer
provider_name: Best Buy
provider_slug: best-buy
schema_file: json-schema/recommendations-api-recommended-product-schema.json
slug: recommendations-api-recommended-product
tags:
- Retail
- Consumer Electronics
- E-Commerce
- Products
- Stores
title: RecommendedProduct
---
