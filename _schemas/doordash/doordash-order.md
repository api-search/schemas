---
description: Represents an order placed through the DoorDash marketplace, including items, customer details, delivery information, and order status.
layout: schema
name: DoorDash Marketplace Order
properties_list:
- description: The unique DoorDash order identifier.
  name: id
  type: string
- description: An external reference ID for the order provided by the partner.
  name: external_reference_id
  type: string
- description: The current status of the order.
  name: status
  type: string
- description: The merchant-supplied store identifier.
  name: store_id
  type: string
- description: The order subtotal in cents.
  name: subtotal
  type: integer
- description: The tax amount in cents.
  name: tax
  type: integer
- description: The delivery fee in cents.
  name: delivery_fee
  type: integer
- description: The tip amount in cents.
  name: tip
  type: integer
- description: The items in the order.
  name: items
  type: array
- description: ''
  name: customer
  type: object
- description: The delivery address for the order.
  name: delivery_address
  type: string
- description: Special instructions from the customer.
  name: special_instructions
  type: string
- description: The estimated time the Dasher will arrive to pick up the order.
  name: estimated_pickup_time
  type: string
- description: When the order was created.
  name: created_at
  type: string
provider_name: doordash
provider_slug: doordash
schema_file: json-schema/doordash-order-schema.json
slug: doordash-order
source_filename: doordash-order-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.doordash.com/schemas/doordash/order.json\",\n  \"title\": \"DoorDash Marketplace Order\",\n  \"description\": \"Represents an order placed through the DoorDash marketplace, including items, customer details, delivery information, and order status.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"id\",\n    \"store_id\",\n    \"items\"\n  ],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique DoorDash order identifier.\"\n    },\n    \"external_reference_id\": {\n      \"type\": \"string\",\n      \"description\": \"An external reference ID for the order provided by the partner.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the order.\",\n      \"enum\": [\n        \"pending\",\n        \"confirmed\",\n        \"being_prepared\",\n        \"ready_for_pickup\",\n \
  \       \"picked_up\",\n        \"delivered\",\n        \"cancelled\"\n      ]\n    },\n    \"store_id\": {\n      \"type\": \"string\",\n      \"description\": \"The merchant-supplied store identifier.\"\n    },\n    \"subtotal\": {\n      \"type\": \"integer\",\n      \"description\": \"The order subtotal in cents.\",\n      \"minimum\": 0\n    },\n    \"tax\": {\n      \"type\": \"integer\",\n      \"description\": \"The tax amount in cents.\",\n      \"minimum\": 0\n    },\n    \"delivery_fee\": {\n      \"type\": \"integer\",\n      \"description\": \"The delivery fee in cents.\",\n      \"minimum\": 0\n    },\n    \"tip\": {\n      \"type\": \"integer\",\n      \"description\": \"The tip amount in cents.\",\n      \"minimum\": 0\n    },\n    \"items\": {\n      \"type\": \"array\",\n      \"description\": \"The items in the order.\",\n      \"minItems\": 1,\n      \"items\": {\n        \"$ref\": \"#/$defs/OrderItem\"\n      }\n    },\n    \"customer\": {\n      \"$ref\": \"#/$defs/Customer\"\
  \n    },\n    \"delivery_address\": {\n      \"type\": \"string\",\n      \"description\": \"The delivery address for the order.\"\n    },\n    \"special_instructions\": {\n      \"type\": \"string\",\n      \"description\": \"Special instructions from the customer.\",\n      \"maxLength\": 500\n    },\n    \"estimated_pickup_time\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The estimated time the Dasher will arrive to pick up the order.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the order was created.\"\n    }\n  },\n  \"$defs\": {\n    \"OrderItem\": {\n      \"type\": \"object\",\n      \"description\": \"An item within a marketplace order.\",\n      \"required\": [\n        \"id\",\n        \"name\",\n        \"quantity\",\n        \"price\"\n      ],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\"\
  : \"The unique item identifier within the order.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the item.\"\n        },\n        \"quantity\": {\n          \"type\": \"integer\",\n          \"description\": \"The quantity ordered.\",\n          \"minimum\": 1\n        },\n        \"price\": {\n          \"type\": \"integer\",\n          \"description\": \"The item price in cents.\",\n          \"minimum\": 0\n        },\n        \"special_instructions\": {\n          \"type\": \"string\",\n          \"description\": \"Special instructions for this item.\",\n          \"maxLength\": 500\n        },\n        \"options\": {\n          \"type\": \"array\",\n          \"description\": \"Selected options or modifiers for the item.\",\n          \"items\": {\n            \"$ref\": \"#/$defs/ItemOption\"\n          }\n        }\n      }\n    },\n    \"ItemOption\": {\n      \"type\": \"object\",\n      \"description\": \"A selected\
  \ option or modifier for an order item.\",\n      \"required\": [\n        \"id\",\n        \"name\"\n      ],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The unique option identifier.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The option name.\"\n        },\n        \"quantity\": {\n          \"type\": \"integer\",\n          \"description\": \"The quantity of this option.\",\n          \"minimum\": 1\n        },\n        \"price\": {\n          \"type\": \"integer\",\n          \"description\": \"The option price in cents.\",\n          \"minimum\": 0\n        }\n      }\n    },\n    \"Customer\": {\n      \"type\": \"object\",\n      \"description\": \"Customer information for the order.\",\n      \"properties\": {\n        \"first_name\": {\n          \"type\": \"string\",\n          \"description\": \"The customer's first name.\"\n        },\n        \"last_name\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"The customer's last name.\"\n        },\n        \"phone_number\": {\n          \"type\": \"string\",\n          \"description\": \"The customer's phone number.\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/doordash/refs/heads/main/json-schema/doordash-order-schema.json
tags: []
title: DoorDash Marketplace Order
---
