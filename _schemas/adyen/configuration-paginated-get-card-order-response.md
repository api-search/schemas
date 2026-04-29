---
description: PaginatedGetCardOrderResponse schema from Adyen API
layout: schema
name: PaginatedGetCardOrderResponse
properties_list:
- description: Contains objects with information about card orders.
  name: cardOrders
  type: array
- description: Indicates whether there are more items on the next page.
  name: hasNext
  type: boolean
- description: Indicates whether there are more items on the previous page.
  name: hasPrevious
  type: boolean
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-paginated-get-card-order-response-schema.json
slug: configuration-paginated-get-card-order-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-paginated-get-card-order-response-schema.json\",\n  \"title\": \"PaginatedGetCardOrderResponse\",\n  \"description\": \"PaginatedGetCardOrderResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cardOrders\": {\n      \"description\": \"Contains objects with information about card orders.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/CardOrder\"\n      },\n      \"type\": \"array\"\n    },\n    \"hasNext\": {\n      \"description\": \"Indicates whether there are more items on the next page.\",\n      \"type\": \"boolean\"\n    },\n    \"hasPrevious\": {\n      \"description\": \"Indicates whether there are more items on the previous page.\",\n      \"type\": \"boolean\"\n    }\n  },\n  \"required\": [\n    \"hasPrevious\",\n    \"hasNext\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-paginated-get-card-order-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PaginatedGetCardOrderResponse
---
