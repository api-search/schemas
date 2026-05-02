---
description: A complete order placed through the Grubhub Marketplace, including items, totals, customer information, delivery address, and lifecycle status.
layout: schema
name: Grubhub Order
properties_list:
- description: The unique identifier for the order.
  name: order_uuid
  type: string
- description: The Grubhub merchant identifier this order was placed with.
  name: merchant_id
  type: string
- description: The partner's external identifier for this order.
  name: external_order_id
  type: string
- description: The current lifecycle status of the order.
  name: status
  type: string
- description: The type of fulfillment for this order.
  name: fulfillment_type
  type: string
- description: The timestamp when the order was placed by the diner.
  name: placed_at
  type: string
- description: The timestamp when the order was confirmed by the merchant.
  name: confirmed_at
  type: string
- description: The estimated delivery or pickup time for the order.
  name: estimated_delivery_at
  type: string
- description: ''
  name: customer
  type: object
- description: The items included in this order.
  name: items
  type: array
- description: ''
  name: totals
  type: object
- description: ''
  name: delivery_address
  type: object
- description: Special instructions provided by the customer for the entire order.
  name: special_instructions
  type: string
- description: Estimated number of minutes until the order is ready, set during confirmation.
  name: wait_time_in_minutes
  type: integer
provider_name: grubhub
provider_slug: grubhub
schema_file: json-schema/grubhub-order-schema.json
slug: grubhub-order
source_filename: grubhub-order-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.grubhub.com/schemas/grubhub/order.json\",\n  \"title\": \"Grubhub Order\",\n  \"description\": \"A complete order placed through the Grubhub Marketplace, including items, totals, customer information, delivery address, and lifecycle status.\",\n  \"type\": \"object\",\n  \"required\": [\"order_uuid\", \"merchant_id\", \"status\", \"items\", \"totals\"],\n  \"properties\": {\n    \"order_uuid\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The unique identifier for the order.\"\n    },\n    \"merchant_id\": {\n      \"type\": \"string\",\n      \"description\": \"The Grubhub merchant identifier this order was placed with.\"\n    },\n    \"external_order_id\": {\n      \"type\": \"string\",\n      \"description\": \"The partner's external identifier for this order.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"The current lifecycle status of the order.\",\n      \"enum\": [\"PENDING\", \"CONFIRMED\", \"IN_PROGRESS\", \"READY\", \"OUT_FOR_DELIVERY\", \"COMPLETED\", \"CANCELLED\"]\n    },\n    \"fulfillment_type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of fulfillment for this order.\",\n      \"enum\": [\"DELIVERY\", \"PICKUP\"]\n    },\n    \"placed_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp when the order was placed by the diner.\"\n    },\n    \"confirmed_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp when the order was confirmed by the merchant.\"\n    },\n    \"estimated_delivery_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The estimated delivery or pickup time for the order.\"\n    },\n    \"customer\": {\n      \"$ref\": \"#/$defs/Customer\"\n    },\n    \"items\": {\n     \
  \ \"type\": \"array\",\n      \"description\": \"The items included in this order.\",\n      \"minItems\": 1,\n      \"items\": {\n        \"$ref\": \"#/$defs/OrderItem\"\n      }\n    },\n    \"totals\": {\n      \"$ref\": \"#/$defs/OrderTotals\"\n    },\n    \"delivery_address\": {\n      \"$ref\": \"#/$defs/Address\"\n    },\n    \"special_instructions\": {\n      \"type\": \"string\",\n      \"description\": \"Special instructions provided by the customer for the entire order.\",\n      \"maxLength\": 500\n    },\n    \"wait_time_in_minutes\": {\n      \"type\": \"integer\",\n      \"description\": \"Estimated number of minutes until the order is ready, set during confirmation.\",\n      \"minimum\": 1\n    }\n  },\n  \"$defs\": {\n    \"Customer\": {\n      \"type\": \"object\",\n      \"description\": \"Customer information associated with an order.\",\n      \"properties\": {\n        \"first_name\": {\n          \"type\": \"string\",\n          \"description\": \"The customer's\
  \ first name.\"\n        },\n        \"last_name\": {\n          \"type\": \"string\",\n          \"description\": \"The customer's last name.\"\n        },\n        \"phone\": {\n          \"type\": \"string\",\n          \"description\": \"The customer's phone number.\"\n        }\n      }\n    },\n    \"OrderItem\": {\n      \"type\": \"object\",\n      \"description\": \"An individual item within an order.\",\n      \"required\": [\"item_id\", \"name\", \"quantity\", \"price\"],\n      \"properties\": {\n        \"item_id\": {\n          \"type\": \"string\",\n          \"description\": \"The unique identifier for the menu item.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The display name of the item.\"\n        },\n        \"quantity\": {\n          \"type\": \"integer\",\n          \"description\": \"The quantity ordered.\",\n          \"minimum\": 1\n        },\n        \"price\": {\n          \"type\": \"number\",\n        \
  \  \"description\": \"The unit price of the item.\",\n          \"minimum\": 0\n        },\n        \"size\": {\n          \"type\": \"string\",\n          \"description\": \"The selected size for this item, if applicable.\"\n        },\n        \"modifiers\": {\n          \"type\": \"array\",\n          \"description\": \"Modifiers applied to this item.\",\n          \"items\": {\n            \"$ref\": \"#/$defs/OrderModifier\"\n          }\n        },\n        \"special_instructions\": {\n          \"type\": \"string\",\n          \"description\": \"Item-level special instructions.\",\n          \"maxLength\": 250\n        }\n      }\n    },\n    \"OrderModifier\": {\n      \"type\": \"object\",\n      \"description\": \"A modifier applied to an ordered item.\",\n      \"required\": [\"name\"],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the modifier.\"\n        },\n        \"price\": {\n          \"type\":\
  \ \"number\",\n          \"description\": \"The additional price for this modifier.\",\n          \"minimum\": 0\n        }\n      }\n    },\n    \"OrderTotals\": {\n      \"type\": \"object\",\n      \"description\": \"Financial totals for an order.\",\n      \"required\": [\"total\"],\n      \"properties\": {\n        \"subtotal\": {\n          \"type\": \"number\",\n          \"description\": \"The subtotal before taxes and fees.\",\n          \"minimum\": 0\n        },\n        \"tax\": {\n          \"type\": \"number\",\n          \"description\": \"The tax amount.\",\n          \"minimum\": 0\n        },\n        \"delivery_fee\": {\n          \"type\": \"number\",\n          \"description\": \"The delivery fee charged.\",\n          \"minimum\": 0\n        },\n        \"tip\": {\n          \"type\": \"number\",\n          \"description\": \"The tip amount.\",\n          \"minimum\": 0\n        },\n        \"total\": {\n          \"type\": \"number\",\n          \"description\":\
  \ \"The total amount for the order.\",\n          \"minimum\": 0\n        }\n      }\n    },\n    \"Address\": {\n      \"type\": \"object\",\n      \"description\": \"A physical address.\",\n      \"properties\": {\n        \"street_address\": {\n          \"type\": \"string\",\n          \"description\": \"The street address line.\"\n        },\n        \"apt_suite\": {\n          \"type\": \"string\",\n          \"description\": \"Apartment or suite number.\"\n        },\n        \"city\": {\n          \"type\": \"string\",\n          \"description\": \"The city name.\"\n        },\n        \"state\": {\n          \"type\": \"string\",\n          \"description\": \"The state abbreviation.\",\n          \"maxLength\": 2\n        },\n        \"zip\": {\n          \"type\": \"string\",\n          \"description\": \"The ZIP code.\",\n          \"pattern\": \"^\\\\d{5}(-\\\\d{4})?$\"\n        },\n        \"latitude\": {\n          \"type\": \"number\",\n          \"description\": \"The latitude\
  \ coordinate.\"\n        },\n        \"longitude\": {\n          \"type\": \"number\",\n          \"description\": \"The longitude coordinate.\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/json-schema/grubhub-order-schema.json
tags: []
title: Grubhub Order
---
