---
description: A fulfillment represents the shipment of one or more items from an order. Fulfillments track the status of delivery and include tracking information from the shipping carrier.
layout: schema
name: Shopify Fulfillment
properties_list:
- description: Unique numeric identifier for the fulfillment
  name: id
  type: integer
- description: The ID of the order this fulfillment belongs to
  name: order_id
  type: integer
- description: The status of the fulfillment
  name: status
  type: string
- description: The name of the shipping carrier
  name: tracking_company
  type:
  - string
  - 'null'
- description: The tracking number provided by the shipping carrier
  name: tracking_number
  type:
  - string
  - 'null'
- description: All tracking numbers for the fulfillment
  name: tracking_numbers
  type: array
- description: The URL to track the shipment
  name: tracking_url
  type:
  - string
  - 'null'
- description: All tracking URLs for the fulfillment
  name: tracking_urls
  type: array
- description: Receipt information if applicable
  name: receipt
  type: object
- description: The fulfillment service identifier
  name: service
  type: string
- description: The delivery status from the carrier
  name: shipment_status
  type:
  - string
  - 'null'
- description: The ID of the location where items were fulfilled from
  name: location_id
  type: integer
- description: The origin address of the fulfillment
  name: origin_address
  type:
  - object
  - 'null'
- description: The line items included in this fulfillment
  name: line_items
  type: array
- description: Whether the customer was notified about this fulfillment
  name: notify_customer
  type: boolean
- description: When the fulfillment was created
  name: created_at
  type: string
- description: When the fulfillment was last updated
  name: updated_at
  type: string
- description: The GraphQL Admin API identifier
  name: admin_graphql_api_id
  type: string
provider_name: Shopify
provider_slug: shopify
schema_file: json-schema/shopify-fulfillment-schema.json
slug: shopify-fulfillment
source_filename: shopify-fulfillment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://shopify.dev/schemas/fulfillment.json\",\n  \"title\": \"Shopify Fulfillment\",\n  \"description\": \"A fulfillment represents the shipment of one or more items from an order. Fulfillments track the status of delivery and include tracking information from the shipping carrier.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique numeric identifier for the fulfillment\"\n    },\n    \"order_id\": {\n      \"type\": \"integer\",\n      \"description\": \"The ID of the order this fulfillment belongs to\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the fulfillment\",\n      \"enum\": [\"pending\", \"open\", \"success\", \"cancelled\", \"error\", \"failure\"]\n    },\n    \"tracking_company\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The name\
  \ of the shipping carrier\"\n    },\n    \"tracking_number\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The tracking number provided by the shipping carrier\"\n    },\n    \"tracking_numbers\": {\n      \"type\": \"array\",\n      \"description\": \"All tracking numbers for the fulfillment\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"tracking_url\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"uri\",\n      \"description\": \"The URL to track the shipment\"\n    },\n    \"tracking_urls\": {\n      \"type\": \"array\",\n      \"description\": \"All tracking URLs for the fulfillment\",\n      \"items\": {\n        \"type\": \"string\",\n        \"format\": \"uri\"\n      }\n    },\n    \"receipt\": {\n      \"type\": \"object\",\n      \"description\": \"Receipt information if applicable\",\n      \"properties\": {\n        \"testcase\": {\n          \"type\": \"boolean\"\n        },\n        \"authorization\"\
  : {\n          \"type\": [\"string\", \"null\"]\n        }\n      }\n    },\n    \"service\": {\n      \"type\": \"string\",\n      \"description\": \"The fulfillment service identifier\"\n    },\n    \"shipment_status\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The delivery status from the carrier\",\n      \"enum\": [\n        \"label_printed\",\n        \"label_purchased\",\n        \"attempted_delivery\",\n        \"ready_for_pickup\",\n        \"picked_up\",\n        \"confirmed\",\n        \"in_transit\",\n        \"out_for_delivery\",\n        \"delivered\",\n        \"failure\",\n        null\n      ]\n    },\n    \"location_id\": {\n      \"type\": \"integer\",\n      \"description\": \"The ID of the location where items were fulfilled from\"\n    },\n    \"origin_address\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"The origin address of the fulfillment\"\n    },\n    \"line_items\": {\n      \"type\": \"array\",\n      \"\
  description\": \"The line items included in this fulfillment\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": { \"type\": \"integer\" },\n          \"variant_id\": { \"type\": [\"integer\", \"null\"] },\n          \"product_id\": { \"type\": [\"integer\", \"null\"] },\n          \"title\": { \"type\": \"string\" },\n          \"quantity\": { \"type\": \"integer\" },\n          \"sku\": { \"type\": [\"string\", \"null\"] },\n          \"price\": { \"type\": \"string\" },\n          \"name\": { \"type\": \"string\" }\n        }\n      }\n    },\n    \"notify_customer\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the customer was notified about this fulfillment\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the fulfillment was created\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"\
  description\": \"When the fulfillment was last updated\"\n    },\n    \"admin_graphql_api_id\": {\n      \"type\": \"string\",\n      \"description\": \"The GraphQL Admin API identifier\"\n    }\n  },\n  \"required\": [\"id\", \"order_id\", \"status\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/shopify/refs/heads/main/json-schema/shopify-fulfillment-schema.json
tags:
- Commerce
- Ecommerce
- Payments
- Retail
- Shopping Cart
- T1
title: Shopify Fulfillment
---
