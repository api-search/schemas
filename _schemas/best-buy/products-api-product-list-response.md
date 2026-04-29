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
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/best-buy/refs/heads/main/json-schema/products-api-product-list-response-schema.json\",\n  \"title\": \"ProductListResponse\",\n  \"description\": \"Paginated list of Best Buy products.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"from\": {\n      \"type\": \"integer\",\n      \"description\": \"Starting index of returned results.\",\n      \"example\": 1\n    },\n    \"to\": {\n      \"type\": \"integer\",\n      \"description\": \"Ending index of returned results.\",\n      \"example\": 10\n    },\n    \"total\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of matching products.\",\n      \"example\": 125000\n    },\n    \"currentPage\": {\n      \"type\": \"integer\",\n      \"description\": \"Current page number.\",\n      \"example\": 1\n    },\n    \"totalPages\": {\n      \"type\": \"integer\",\n      \"\
  description\": \"Total number of pages available.\",\n      \"example\": 12500\n    },\n    \"queryTime\": {\n      \"type\": \"string\",\n      \"description\": \"Time taken to execute the query in seconds.\",\n      \"example\": \"0.023\"\n    },\n    \"totalTime\": {\n      \"type\": \"string\",\n      \"description\": \"Total response time in seconds.\",\n      \"example\": \"0.043\"\n    },\n    \"partial\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the response is a partial result.\",\n      \"example\": false\n    },\n    \"canonicalUrl\": {\n      \"type\": \"string\",\n      \"description\": \"The canonical URL for this query.\",\n      \"example\": \"https://api.bestbuy.com/v1/products?format=json&pageSize=10\"\n    },\n    \"nextCursorMark\": {\n      \"type\": \"string\",\n      \"description\": \"Cursor mark for fetching the next page when using cursor-based pagination.\",\n      \"example\": \"AoE=\"\n    },\n    \"products\": {\n      \"type\": \"\
  array\",\n      \"description\": \"Array of product objects.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Product\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/best-buy/refs/heads/main/json-schema/products-api-product-list-response-schema.json
tags:
- Retail
- Consumer Electronics
- E-Commerce
- Products
- Stores
title: ProductListResponse
---
