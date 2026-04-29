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
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/best-buy/refs/heads/main/json-schema/stores-api-store-list-response-schema.json\",\n  \"title\": \"StoreListResponse\",\n  \"description\": \"Paginated list of Best Buy store locations.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"from\": {\n      \"type\": \"integer\",\n      \"description\": \"Starting index of returned results.\",\n      \"example\": 1\n    },\n    \"to\": {\n      \"type\": \"integer\",\n      \"description\": \"Ending index of returned results.\",\n      \"example\": 5\n    },\n    \"total\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of matching stores.\",\n      \"example\": 1587\n    },\n    \"currentPage\": {\n      \"type\": \"integer\",\n      \"description\": \"Current page number.\",\n      \"example\": 1\n    },\n    \"totalPages\": {\n      \"type\": \"integer\",\n      \"description\"\
  : \"Total number of pages available.\",\n      \"example\": 159\n    },\n    \"queryTime\": {\n      \"type\": \"string\",\n      \"description\": \"Time taken to execute the query in seconds.\",\n      \"example\": \"0.018\"\n    },\n    \"totalTime\": {\n      \"type\": \"string\",\n      \"description\": \"Total response time in seconds.\",\n      \"example\": \"0.032\"\n    },\n    \"stores\": {\n      \"type\": \"array\",\n      \"description\": \"Array of store objects.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Store\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/best-buy/refs/heads/main/json-schema/stores-api-store-list-response-schema.json
tags:
- Retail
- Consumer Electronics
- E-Commerce
- Products
- Stores
title: StoreListResponse
---
