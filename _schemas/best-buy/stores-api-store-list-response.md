---
description: Paginated list of Best Buy store locations.
layout: schema
name: StoreListResponse
properties_list:
- description: Starting index of returned results.
  name: from
  type: integer
- description: Ending index of returned results.
  name: to
  type: integer
- description: Total number of matching stores.
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
- description: Array of store objects.
  name: stores
  type: array
provider_name: Best Buy
provider_slug: best-buy
schema_file: json-schema/stores-api-store-list-response-schema.json
slug: stores-api-store-list-response
tags:
- Retail
- Consumer Electronics
- E-Commerce
- Products
- Stores
title: StoreListResponse
---
