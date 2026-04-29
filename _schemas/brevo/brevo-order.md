---
description: Represents an eCommerce order synced to the Brevo platform for revenue attribution, purchase behavior tracking, and automated marketing workflows.
layout: schema
name: Brevo eCommerce Order
properties_list:
- description: Unique identifier of the order from the merchant's system.
  name: id
  type: string
- description: Email address of the customer who placed the order.
  name: email
  type: string
- description: Current status of the order in the fulfillment workflow.
  name: status
  type: string
- description: Total order amount including shipping, tax, and item prices.
  name: amount
  type: number
- description: List of products included in the order.
  name: products
  type: array
- description: UTC date-time when the order was created.
  name: createdAt
  type: string
- description: UTC date-time when the order was last updated.
  name: updatedAt
  type: string
- description: Coupon codes applied to the order.
  name: coupons
  type: array
provider_name: brevo
provider_slug: brevo
schema_file: json-schema/brevo-order-schema.json
slug: brevo-order
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://brevo.com/schemas/brevo/order.json\",\n  \"title\": \"Brevo eCommerce Order\",\n  \"description\": \"Represents an eCommerce order synced to the Brevo platform for revenue attribution, purchase behavior tracking, and automated marketing workflows.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"email\", \"status\", \"amount\", \"products\", \"createdAt\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the order from the merchant's system.\",\n      \"minLength\": 1\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Email address of the customer who placed the order.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current status of the order in the fulfillment workflow.\",\n      \"enum\": [\"pending\", \"completed\", \"\
  cancelled\", \"refunded\", \"shipped\", \"processing\"]\n    },\n    \"amount\": {\n      \"type\": \"number\",\n      \"description\": \"Total order amount including shipping, tax, and item prices.\",\n      \"minimum\": 0\n    },\n    \"products\": {\n      \"type\": \"array\",\n      \"description\": \"List of products included in the order.\",\n      \"minItems\": 1,\n      \"items\": {\n        \"$ref\": \"#/$defs/OrderProduct\"\n      }\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"UTC date-time when the order was created.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"UTC date-time when the order was last updated.\"\n    },\n    \"coupons\": {\n      \"type\": \"array\",\n      \"description\": \"Coupon codes applied to the order.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"OrderProduct\"\
  : {\n      \"type\": \"object\",\n      \"description\": \"Represents a product line item within an eCommerce order.\",\n      \"required\": [\"productId\", \"quantity\", \"price\"],\n      \"properties\": {\n        \"productId\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier of the product.\",\n          \"minLength\": 1\n        },\n        \"quantity\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of units of the product ordered.\",\n          \"minimum\": 1\n        },\n        \"price\": {\n          \"type\": \"number\",\n          \"description\": \"Unit price of the product at the time of the order.\",\n          \"minimum\": 0\n        },\n        \"variantId\": {\n          \"type\": \"string\",\n          \"description\": \"Variant identifier if the product has size, color, or other variants.\"\n        }\n      }\n    },\n    \"Product\": {\n      \"type\": \"object\",\n      \"description\": \"Represents a product\
  \ in the Brevo eCommerce catalog.\",\n      \"required\": [\"id\", \"name\", \"url\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier of the product.\",\n          \"minLength\": 1\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the product.\",\n          \"minLength\": 1\n        },\n        \"url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL of the product page on the merchant's website.\"\n        },\n        \"imageUrl\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL of the product image.\"\n        },\n        \"sku\": {\n          \"type\": \"string\",\n          \"description\": \"Stock keeping unit identifier for inventory tracking.\"\n        },\n        \"price\": {\n          \"type\": \"number\",\n          \"description\": \"Current\
  \ price of the product.\",\n          \"minimum\": 0\n        },\n        \"categories\": {\n          \"type\": \"array\",\n          \"description\": \"IDs of categories the product belongs to.\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"metaInfo\": {\n          \"type\": \"object\",\n          \"description\": \"Additional metadata about the product as key-value pairs.\",\n          \"additionalProperties\": true\n        }\n      }\n    },\n    \"Category\": {\n      \"type\": \"object\",\n      \"description\": \"Represents a product category in the Brevo eCommerce catalog.\",\n      \"required\": [\"id\", \"name\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier of the category.\",\n          \"minLength\": 1\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the category.\",\n          \"minLength\"\
  : 1\n        },\n        \"url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL of the category page on the merchant's website.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/brevo/refs/heads/main/json-schema/brevo-order-schema.json
tags: []
title: Brevo eCommerce Order
---
