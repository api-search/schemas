---
description: Order schema from Amazon Selling Partner API
layout: schema
name: Order
properties_list:
- description: ''
  name: AmazonOrderId
  type: string
- description: ''
  name: PurchaseDate
  type: string
- description: ''
  name: LastUpdateDate
  type: string
- description: ''
  name: OrderStatus
  type: string
- description: ''
  name: FulfillmentChannel
  type: string
- description: ''
  name: OrderTotal
  type: object
- description: ''
  name: NumberOfItemsShipped
  type: integer
- description: ''
  name: NumberOfItemsUnshipped
  type: integer
- description: ''
  name: ShipServiceLevel
  type: string
- description: ''
  name: MarketplaceId
  type: string
provider_name: Amazon
provider_slug: amazon
schema_file: json-schema/selling-partner-order-schema.json
slug: selling-partner-order
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"AmazonOrderId\": {\n      \"type\": \"string\"\n    },\n    \"PurchaseDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"LastUpdateDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"OrderStatus\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Pending\",\n        \"Unshipped\",\n        \"PartiallyShipped\",\n        \"Shipped\",\n        \"Canceled\",\n        \"Unfulfillable\"\n      ]\n    },\n    \"FulfillmentChannel\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"MFN\",\n        \"AFN\"\n      ]\n    },\n    \"OrderTotal\": {\n      \"$ref\": \"#/components/schemas/Money\"\n    },\n    \"NumberOfItemsShipped\": {\n      \"type\": \"integer\"\n    },\n    \"NumberOfItemsUnshipped\": {\n      \"type\": \"integer\"\n    },\n    \"ShipServiceLevel\": {\n      \"type\": \"string\"\n    },\n    \"MarketplaceId\": {\n   \
  \   \"type\": \"string\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Order\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/json-schema/selling-partner-order-schema.json\",\n  \"description\": \"Order schema from Amazon Selling Partner API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/json-schema/selling-partner-order-schema.json
tags:
- Amazon
- Advertising
- Alexa
- E-Commerce
- Marketplace
- Payments
- Voice
title: Order
---
