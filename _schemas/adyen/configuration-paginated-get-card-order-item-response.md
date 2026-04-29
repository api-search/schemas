---
description: PaginatedGetCardOrderItemResponse schema from Adyen API
layout: schema
name: PaginatedGetCardOrderItemResponse
properties_list:
- description: List of card order items in the card order batch.
  name: data
  type: array
- description: Indicates whether there are more items on the next page.
  name: hasNext
  type: boolean
- description: Indicates whether there are more items on the previous page.
  name: hasPrevious
  type: boolean
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-paginated-get-card-order-item-response-schema.json
slug: configuration-paginated-get-card-order-item-response
source_filename: configuration-paginated-get-card-order-item-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-paginated-get-card-order-item-response-schema.json\",\n  \"title\": \"PaginatedGetCardOrderItemResponse\",\n  \"description\": \"PaginatedGetCardOrderItemResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"description\": \"List of card order items in the card order batch.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/CardOrderItem\"\n      },\n      \"type\": \"array\"\n    },\n    \"hasNext\": {\n      \"description\": \"Indicates whether there are more items on the next page.\",\n      \"type\": \"boolean\"\n    },\n    \"hasPrevious\": {\n      \"description\": \"Indicates whether there are more items on the previous page.\",\n      \"type\": \"boolean\"\n    }\n  },\n  \"required\": [\n    \"data\",\n    \"hasPrevious\",\n\
  \    \"hasNext\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-paginated-get-card-order-item-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PaginatedGetCardOrderItemResponse
---
