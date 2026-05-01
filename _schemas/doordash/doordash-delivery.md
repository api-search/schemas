---
description: Represents a delivery fulfilled by DoorDash's fleet of Dashers, including pickup and dropoff details, status tracking, and Dasher assignment information.
layout: schema
name: DoorDash Delivery
properties_list:
- description: A unique identifier for this delivery, provided by the caller.
  name: external_delivery_id
  type: string
- description: The current status of the delivery as it progresses through the lifecycle.
  name: delivery_status
  type: string
- description: The delivery fee in cents.
  name: fee
  type: integer
- description: The ISO 4217 currency code for monetary amounts.
  name: currency
  type: string
- description: The tip amount in cents.
  name: tip
  type: integer
- description: The total value of the order in cents.
  name: order_value
  type: integer
- description: The full street address for the pickup location.
  name: pickup_address
  type: string
- description: The business name at the pickup location.
  name: pickup_business_name
  type: string
- description: The phone number at the pickup location.
  name: pickup_phone_number
  type: string
- description: Special instructions for the Dasher at the pickup location.
  name: pickup_instructions
  type: string
- description: A reference tag for the pickup, such as an order number.
  name: pickup_reference_tag
  type: string
- description: The estimated pickup time in UTC ISO-8601 format.
  name: pickup_time_estimated
  type: string
- description: The actual pickup time in UTC ISO-8601 format.
  name: pickup_time_actual
  type: string
- description: The full street address for the dropoff location.
  name: dropoff_address
  type: string
- description: The business name at the dropoff location.
  name: dropoff_business_name
  type: string
- description: The phone number of the recipient at the dropoff location.
  name: dropoff_phone_number
  type: string
- description: Special instructions for the Dasher at the dropoff location.
  name: dropoff_instructions
  type: string
- description: The first name of the dropoff contact.
  name: dropoff_contact_given_name
  type: string
- description: The last name of the dropoff contact.
  name: dropoff_contact_family_name
  type: string
- description: The estimated dropoff time in UTC ISO-8601 format.
  name: dropoff_time_estimated
  type: string
- description: The actual dropoff time in UTC ISO-8601 format.
  name: dropoff_time_actual
  type: string
- description: Whether the order contains alcohol, requiring age verification.
  name: contains_alcohol
  type: boolean
- description: An identifier to group deliveries for batch assignment to the same Dasher.
  name: force_batch_id
  type: string
- description: ''
  name: dasher
  type: object
- description: A URL for tracking the delivery in real time.
  name: tracking_url
  type: string
- description: List of items included in the delivery.
  name: items
  type: array
- description: The external business ID associated with this delivery.
  name: external_business_id
  type: string
- description: The external store ID associated with this delivery.
  name: external_store_id
  type: string
- description: The timestamp when the delivery was created.
  name: created_at
  type: string
- description: The timestamp when the delivery was last updated.
  name: updated_at
  type: string
provider_name: doordash
provider_slug: doordash
schema_file: json-schema/doordash-delivery-schema.json
slug: doordash-delivery
source_filename: doordash-delivery-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.doordash.com/schemas/doordash/delivery.json\",\n  \"title\": \"DoorDash Delivery\",\n  \"description\": \"Represents a delivery fulfilled by DoorDash's fleet of Dashers, including pickup and dropoff details, status tracking, and Dasher assignment information.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"external_delivery_id\",\n    \"pickup_address\",\n    \"dropoff_address\"\n  ],\n  \"properties\": {\n    \"external_delivery_id\": {\n      \"type\": \"string\",\n      \"description\": \"A unique identifier for this delivery, provided by the caller.\",\n      \"minLength\": 1\n    },\n    \"delivery_status\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the delivery as it progresses through the lifecycle.\",\n      \"enum\": [\n        \"created\",\n        \"confirmed\",\n        \"enroute_to_pickup\",\n        \"arrived_at_pickup\"\
  ,\n        \"picked_up\",\n        \"enroute_to_dropoff\",\n        \"arrived_at_dropoff\",\n        \"delivered\",\n        \"cancelled\",\n        \"returned\"\n      ]\n    },\n    \"fee\": {\n      \"type\": \"integer\",\n      \"description\": \"The delivery fee in cents.\",\n      \"minimum\": 0\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"The ISO 4217 currency code for monetary amounts.\",\n      \"pattern\": \"^[A-Z]{3}$\"\n    },\n    \"tip\": {\n      \"type\": \"integer\",\n      \"description\": \"The tip amount in cents.\",\n      \"minimum\": 0\n    },\n    \"order_value\": {\n      \"type\": \"integer\",\n      \"description\": \"The total value of the order in cents.\",\n      \"minimum\": 0\n    },\n    \"pickup_address\": {\n      \"type\": \"string\",\n      \"description\": \"The full street address for the pickup location.\"\n    },\n    \"pickup_business_name\": {\n      \"type\": \"string\",\n      \"description\": \"The business\
  \ name at the pickup location.\"\n    },\n    \"pickup_phone_number\": {\n      \"type\": \"string\",\n      \"description\": \"The phone number at the pickup location.\"\n    },\n    \"pickup_instructions\": {\n      \"type\": \"string\",\n      \"description\": \"Special instructions for the Dasher at the pickup location.\"\n    },\n    \"pickup_reference_tag\": {\n      \"type\": \"string\",\n      \"description\": \"A reference tag for the pickup, such as an order number.\"\n    },\n    \"pickup_time_estimated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The estimated pickup time in UTC ISO-8601 format.\"\n    },\n    \"pickup_time_actual\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The actual pickup time in UTC ISO-8601 format.\"\n    },\n    \"dropoff_address\": {\n      \"type\": \"string\",\n      \"description\": \"The full street address for the dropoff location.\"\n    },\n    \"\
  dropoff_business_name\": {\n      \"type\": \"string\",\n      \"description\": \"The business name at the dropoff location.\"\n    },\n    \"dropoff_phone_number\": {\n      \"type\": \"string\",\n      \"description\": \"The phone number of the recipient at the dropoff location.\"\n    },\n    \"dropoff_instructions\": {\n      \"type\": \"string\",\n      \"description\": \"Special instructions for the Dasher at the dropoff location.\"\n    },\n    \"dropoff_contact_given_name\": {\n      \"type\": \"string\",\n      \"description\": \"The first name of the dropoff contact.\"\n    },\n    \"dropoff_contact_family_name\": {\n      \"type\": \"string\",\n      \"description\": \"The last name of the dropoff contact.\"\n    },\n    \"dropoff_time_estimated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The estimated dropoff time in UTC ISO-8601 format.\"\n    },\n    \"dropoff_time_actual\": {\n      \"type\": \"string\",\n      \"format\"\
  : \"date-time\",\n      \"description\": \"The actual dropoff time in UTC ISO-8601 format.\"\n    },\n    \"contains_alcohol\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the order contains alcohol, requiring age verification.\"\n    },\n    \"force_batch_id\": {\n      \"type\": \"string\",\n      \"description\": \"An identifier to group deliveries for batch assignment to the same Dasher.\"\n    },\n    \"dasher\": {\n      \"$ref\": \"#/$defs/Dasher\"\n    },\n    \"tracking_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"A URL for tracking the delivery in real time.\"\n    },\n    \"items\": {\n      \"type\": \"array\",\n      \"description\": \"List of items included in the delivery.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/DeliveryItem\"\n      }\n    },\n    \"external_business_id\": {\n      \"type\": \"string\",\n      \"description\": \"The external business ID associated with this delivery.\"\n  \
  \  },\n    \"external_store_id\": {\n      \"type\": \"string\",\n      \"description\": \"The external store ID associated with this delivery.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp when the delivery was created.\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp when the delivery was last updated.\"\n    }\n  },\n  \"$defs\": {\n    \"Dasher\": {\n      \"type\": \"object\",\n      \"description\": \"Information about the Dasher assigned to fulfill the delivery.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\",\n          \"description\": \"The unique identifier for the Dasher.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The first name of the Dasher.\"\n        },\n        \"phone_number\": {\n          \"type\": \"string\"\
  ,\n          \"description\": \"The phone number of the Dasher.\"\n        },\n        \"location\": {\n          \"$ref\": \"#/$defs/Location\"\n        }\n      }\n    },\n    \"Location\": {\n      \"type\": \"object\",\n      \"description\": \"A geographic coordinate point.\",\n      \"properties\": {\n        \"lat\": {\n          \"type\": \"number\",\n          \"format\": \"double\",\n          \"description\": \"Latitude coordinate.\",\n          \"minimum\": -90,\n          \"maximum\": 90\n        },\n        \"lng\": {\n          \"type\": \"number\",\n          \"format\": \"double\",\n          \"description\": \"Longitude coordinate.\",\n          \"minimum\": -180,\n          \"maximum\": 180\n        }\n      },\n      \"required\": [\n        \"lat\",\n        \"lng\"\n      ]\n    },\n    \"DeliveryItem\": {\n      \"type\": \"object\",\n      \"description\": \"An item included in a delivery.\",\n      \"required\": [\n        \"name\",\n        \"quantity\"\n    \
  \  ],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the item.\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"A description of the item.\"\n        },\n        \"quantity\": {\n          \"type\": \"integer\",\n          \"description\": \"The quantity of this item.\",\n          \"minimum\": 1\n        },\n        \"external_id\": {\n          \"type\": \"string\",\n          \"description\": \"An external identifier for the item.\"\n        },\n        \"price\": {\n          \"type\": \"integer\",\n          \"description\": \"The price of the item in cents.\",\n          \"minimum\": 0\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/doordash/refs/heads/main/json-schema/doordash-delivery-schema.json
tags: []
title: DoorDash Delivery
---
