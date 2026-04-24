---
description: Paginated list of Best Buy products.
layout: schema
name: ProductListResponse
properties_list:
- description: Starting index of returned results.
  name: from
  type: integer
- description: Ending index of returned results.
  name: to
  type: integer
- description: Total number of matching products.
  name: total
  type: integer
- description: Current page number.
  name: currentPage
  type: integer
- description: Total number of pages available.
  name: totalPages
  type: integer
- description: Time taken to execute the query in seconds.
  name: queryTime
  type: string
- description: Total response time in seconds.
  name: totalTime
  type: string
- description: Whether the response is a partial result.
  name: partial
  type: boolean
- description: The canonical URL for this query.
  name: canonicalUrl
  type: string
- description: Cursor mark for fetching the next page when using cursor-based pagination.
  name: nextCursorMark
  type: string
- description: Array of product objects.
  name: products
  type: array
provider_name: Best Buy
provider_slug: best-buy
schema_file: json-schema/products-api-product-list-response-schema.json
slug: products-api-product-list-response
tags:
- Retail
- Consumer Electronics
- E-Commerce
- Products
- Stores
title: ProductListResponse
---
