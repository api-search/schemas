---
description: Represents an order in the Instacart Connect system, covering delivery, pickup, and last mile fulfillment types with their associated items, service options, and status lifecycle.
layout: schema
name: Instacart Order
properties_list:
- description: The unique identifier for the order.
  name: id
  type: string
- description: The retailer's unique identifier for the customer who placed the order.
  name: user_id
  type: string
- description: The current status of the order in the fulfillment lifecycle.
  name: status
  type: string
- description: The type of fulfillment for this order.
  name: fulfillment_type
  type: string
- description: The timestamp when the order was created.
  name: created_at
  type: string
- description: The estimated delivery or pickup time.
  name: estimated_delivery_at
  type: string
- description: ''
  name: store
  type: object
- description: ''
  name: service_option
  type: object
- description: ''
  name: delivery_address
  type: object
- description: Special instructions for the delivery driver or pickup process.
  name: delivery_instructions
  type: string
- description: The items included in the order.
  name: items
  type: array
- description: ''
  name: shopper
  type: object
provider_name: instacart
provider_slug: instacart
schema_file: json-schema/instacart-order-schema.json
slug: instacart-order
source_filename: instacart-order-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://instacart.com/schemas/instacart/order.json\",\n  \"title\": \"Instacart Order\",\n  \"description\": \"Represents an order in the Instacart Connect system, covering delivery, pickup, and last mile fulfillment types with their associated items, service options, and status lifecycle.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"status\", \"fulfillment_type\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the order.\"\n    },\n    \"user_id\": {\n      \"type\": \"string\",\n      \"description\": \"The retailer's unique identifier for the customer who placed the order.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"brand_new\",\n        \"acknowledged\",\n        \"picking\",\n        \"staging\",\n        \"delivering\",\n        \"delivered\",\n        \"canceled\"\
  ,\n        \"rescheduled\"\n      ],\n      \"description\": \"The current status of the order in the fulfillment lifecycle.\"\n    },\n    \"fulfillment_type\": {\n      \"type\": \"string\",\n      \"enum\": [\"delivery\", \"pickup\", \"last_mile\"],\n      \"description\": \"The type of fulfillment for this order.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp when the order was created.\"\n    },\n    \"estimated_delivery_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The estimated delivery or pickup time.\"\n    },\n    \"store\": {\n      \"$ref\": \"#/$defs/Store\"\n    },\n    \"service_option\": {\n      \"$ref\": \"#/$defs/ServiceOption\"\n    },\n    \"delivery_address\": {\n      \"$ref\": \"#/$defs/Address\"\n    },\n    \"delivery_instructions\": {\n      \"type\": \"string\",\n      \"description\": \"Special instructions for the delivery\
  \ driver or pickup process.\"\n    },\n    \"items\": {\n      \"type\": \"array\",\n      \"description\": \"The items included in the order.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/OrderItem\"\n      }\n    },\n    \"shopper\": {\n      \"$ref\": \"#/$defs/Shopper\"\n    }\n  },\n  \"$defs\": {\n    \"Store\": {\n      \"type\": \"object\",\n      \"description\": \"A retail store on the Instacart platform.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The unique identifier for the store.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the store.\"\n        },\n        \"address\": {\n          \"$ref\": \"#/$defs/Address\"\n        }\n      }\n    },\n    \"ServiceOption\": {\n      \"type\": \"object\",\n      \"description\": \"A fulfillment time slot selected for the order.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"\
  string\",\n          \"description\": \"The unique identifier for the service option.\"\n        },\n        \"date\": {\n          \"type\": \"string\",\n          \"format\": \"date\",\n          \"description\": \"The date of the service option.\"\n        },\n        \"window_starts_at\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The start time of the fulfillment window.\"\n        },\n        \"window_ends_at\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The end time of the fulfillment window.\"\n        },\n        \"fulfillment_type\": {\n          \"type\": \"string\",\n          \"enum\": [\"delivery\", \"pickup\", \"last_mile\"],\n          \"description\": \"The fulfillment type for this service option.\"\n        }\n      }\n    },\n    \"Address\": {\n      \"type\": \"object\",\n      \"description\": \"A physical address.\",\n      \"properties\": {\n\
  \        \"address_line_1\": {\n          \"type\": \"string\",\n          \"description\": \"The street address.\"\n        },\n        \"address_line_2\": {\n          \"type\": \"string\",\n          \"description\": \"Additional address information such as apartment or suite number.\"\n        },\n        \"city\": {\n          \"type\": \"string\",\n          \"description\": \"The city.\"\n        },\n        \"state\": {\n          \"type\": \"string\",\n          \"description\": \"The state or province.\"\n        },\n        \"postal_code\": {\n          \"type\": \"string\",\n          \"description\": \"The postal or ZIP code.\"\n        },\n        \"latitude\": {\n          \"type\": \"number\",\n          \"description\": \"The latitude coordinate.\"\n        },\n        \"longitude\": {\n          \"type\": \"number\",\n          \"description\": \"The longitude coordinate.\"\n        }\n      }\n    },\n    \"OrderItem\": {\n      \"type\": \"object\",\n      \"description\"\
  : \"An item within an order.\",\n      \"required\": [\"product_id\"],\n      \"properties\": {\n        \"product_id\": {\n          \"type\": \"string\",\n          \"description\": \"The Instacart product identifier.\"\n        },\n        \"upc\": {\n          \"type\": \"string\",\n          \"description\": \"The Universal Product Code.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The display name of the product.\"\n        },\n        \"quantity\": {\n          \"type\": \"integer\",\n          \"description\": \"The ordered quantity.\",\n          \"minimum\": 1\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"enum\": [\"pending\", \"found\", \"replaced\", \"refunded\", \"not_found\"],\n          \"description\": \"The current status of the item during fulfillment.\"\n        },\n        \"replacement\": {\n          \"$ref\": \"#/$defs/Replacement\"\n        },\n        \"replacement_status\"\
  : {\n          \"type\": \"string\",\n          \"enum\": [\"PENDING\", \"APPROVED\", \"REJECTED\"],\n          \"description\": \"The customer's decision on a suggested replacement.\"\n        },\n        \"refunded\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether this item has been refunded.\"\n        }\n      }\n    },\n    \"Replacement\": {\n      \"type\": \"object\",\n      \"description\": \"A replacement product suggested by the shopper.\",\n      \"properties\": {\n        \"product_id\": {\n          \"type\": \"string\",\n          \"description\": \"The product identifier of the replacement.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the replacement product.\"\n        },\n        \"quantity\": {\n          \"type\": \"integer\",\n          \"description\": \"The quantity of the replacement.\",\n          \"minimum\": 1\n        }\n      }\n    },\n    \"Shopper\": {\n      \"type\"\
  : \"object\",\n      \"description\": \"The Instacart shopper assigned to fulfill the order.\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The first name of the shopper.\"\n        },\n        \"phone_number\": {\n          \"type\": \"string\",\n          \"description\": \"A masked phone number for contacting the shopper.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/instacart/refs/heads/main/json-schema/instacart-order-schema.json
tags: []
title: Instacart Order
---
