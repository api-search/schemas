---
description: Represents a booking order on Booking.com, including accommodation reservations, guest details, pricing, cancellation policies, and order lifecycle status.
layout: schema
name: Booking.com Order
properties_list:
- description: Unique identifier for the booking order
  name: order_id
  type: string
- description: Current status of the order
  name: status
  type: string
- description: Identifier of the booked accommodation
  name: accommodation_id
  type: integer
- description: Name of the booked accommodation
  name: accommodation_name
  type: string
- description: Check-in date in YYYY-MM-DD format
  name: checkin
  type: string
- description: Check-out date in YYYY-MM-DD format
  name: checkout
  type: string
- description: ''
  name: booker
  type: object
- description: ''
  name: guests
  type: object
- description: Products (rooms/rates) included in the order
  name: products
  type: array
- description: ''
  name: total_price
  type: object
- description: ''
  name: payment
  type: object
- description: ''
  name: cancellation_policy
  type: object
- description: Any special requests from the guest
  name: special_requests
  type: string
- description: Timestamp when the order was created
  name: created_at
  type: string
- description: Timestamp when the order was last modified
  name: modified_at
  type: string
- description: Timestamp when the order was cancelled, if applicable
  name: cancelled_at
  type: string
provider_name: booking-com
provider_slug: booking-com
schema_file: json-schema/booking-com-order-schema.json
slug: booking-com-order
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://booking.com/schemas/booking-com/order.json\",\n  \"title\": \"Booking.com Order\",\n  \"description\": \"Represents a booking order on Booking.com, including accommodation reservations, guest details, pricing, cancellation policies, and order lifecycle status.\",\n  \"type\": \"object\",\n  \"required\": [\"order_id\", \"status\", \"accommodation_id\", \"checkin\", \"checkout\"],\n  \"properties\": {\n    \"order_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the booking order\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current status of the order\",\n      \"enum\": [\"pending\", \"confirmed\", \"cancelled\", \"modified\", \"completed\", \"no_show\"]\n    },\n    \"accommodation_id\": {\n      \"type\": \"integer\",\n      \"description\": \"Identifier of the booked accommodation\"\n    },\n    \"accommodation_name\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Name of the booked accommodation\"\n    },\n    \"checkin\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Check-in date in YYYY-MM-DD format\"\n    },\n    \"checkout\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Check-out date in YYYY-MM-DD format\"\n    },\n    \"booker\": {\n      \"$ref\": \"#/$defs/Booker\"\n    },\n    \"guests\": {\n      \"$ref\": \"#/$defs/GuestAllocation\"\n    },\n    \"products\": {\n      \"type\": \"array\",\n      \"description\": \"Products (rooms/rates) included in the order\",\n      \"items\": {\n        \"$ref\": \"#/$defs/BookedProduct\"\n      }\n    },\n    \"total_price\": {\n      \"$ref\": \"#/$defs/Price\"\n    },\n    \"payment\": {\n      \"$ref\": \"#/$defs/PaymentSummary\"\n    },\n    \"cancellation_policy\": {\n      \"$ref\": \"#/$defs/CancellationPolicy\"\n    },\n    \"special_requests\": {\n\
  \      \"type\": \"string\",\n      \"description\": \"Any special requests from the guest\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the order was created\"\n    },\n    \"modified_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the order was last modified\"\n    },\n    \"cancelled_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the order was cancelled, if applicable\"\n    }\n  },\n  \"$defs\": {\n    \"Booker\": {\n      \"type\": \"object\",\n      \"description\": \"Person who made the booking\",\n      \"required\": [\"first_name\", \"last_name\", \"email\"],\n      \"properties\": {\n        \"first_name\": {\n          \"type\": \"string\",\n          \"description\": \"Booker first name\",\n          \"minLength\": 1\n        },\n        \"last_name\": {\n \
  \         \"type\": \"string\",\n          \"description\": \"Booker last name\",\n          \"minLength\": 1\n        },\n        \"email\": {\n          \"type\": \"string\",\n          \"format\": \"email\",\n          \"description\": \"Booker email address\"\n        },\n        \"telephone\": {\n          \"type\": \"string\",\n          \"description\": \"Booker telephone number\"\n        },\n        \"country\": {\n          \"type\": \"string\",\n          \"description\": \"Booker country code (ISO 3166-1 alpha-2)\",\n          \"pattern\": \"^[a-z]{2}$\"\n        },\n        \"platform\": {\n          \"type\": \"string\",\n          \"description\": \"Platform the booking was made from\",\n          \"enum\": [\"desktop\", \"mobile\", \"tablet\"]\n        }\n      }\n    },\n    \"GuestAllocation\": {\n      \"type\": \"object\",\n      \"description\": \"Guest allocation for the booking\",\n      \"required\": [\"number_of_adults\", \"number_of_rooms\"],\n      \"properties\"\
  : {\n        \"number_of_adults\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of adult guests\",\n          \"minimum\": 1\n        },\n        \"number_of_rooms\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of rooms booked\",\n          \"minimum\": 1\n        },\n        \"children_ages\": {\n          \"type\": \"array\",\n          \"description\": \"Ages of children in the booking\",\n          \"items\": {\n            \"type\": \"integer\",\n            \"minimum\": 0,\n            \"maximum\": 17\n          }\n        }\n      }\n    },\n    \"BookedProduct\": {\n      \"type\": \"object\",\n      \"description\": \"A room/rate product included in the booking\",\n      \"required\": [\"product_id\"],\n      \"properties\": {\n        \"product_id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique product identifier\"\n        },\n        \"room_name\": {\n          \"type\": \"string\",\n      \
  \    \"description\": \"Name of the booked room type\"\n        },\n        \"meal_plan\": {\n          \"type\": \"string\",\n          \"description\": \"Included meal plan\",\n          \"enum\": [\"room_only\", \"breakfast_included\", \"half_board\", \"full_board\", \"all_inclusive\"]\n        },\n        \"cancellation_type\": {\n          \"type\": \"string\",\n          \"description\": \"Cancellation policy type for this product\"\n        },\n        \"price\": {\n          \"$ref\": \"#/$defs/Price\"\n        },\n        \"quantity\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of this product booked\",\n          \"minimum\": 1\n        }\n      }\n    },\n    \"Price\": {\n      \"type\": \"object\",\n      \"description\": \"Monetary amount with currency\",\n      \"required\": [\"amount\", \"currency\"],\n      \"properties\": {\n        \"amount\": {\n          \"type\": \"number\",\n          \"description\": \"Numeric price amount\",\n    \
  \      \"minimum\": 0\n        },\n        \"currency\": {\n          \"type\": \"string\",\n          \"description\": \"ISO 4217 currency code\",\n          \"pattern\": \"^[A-Z]{3}$\"\n        }\n      }\n    },\n    \"PaymentSummary\": {\n      \"type\": \"object\",\n      \"description\": \"Summary of payment information for the order\",\n      \"properties\": {\n        \"payment_type\": {\n          \"type\": \"string\",\n          \"description\": \"Payment method used\"\n        },\n        \"payment_status\": {\n          \"type\": \"string\",\n          \"description\": \"Current payment status\",\n          \"enum\": [\"pending\", \"paid\", \"refunded\", \"partially_refunded\"]\n        },\n        \"paid_amount\": {\n          \"$ref\": \"#/$defs/Price\"\n        }\n      }\n    },\n    \"CancellationPolicy\": {\n      \"type\": \"object\",\n      \"description\": \"Cancellation policy details for the order\",\n      \"properties\": {\n        \"free_cancellation_until\":\
  \ {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Deadline for free cancellation\"\n        },\n        \"cancellation_fee\": {\n          \"$ref\": \"#/$defs/Price\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"Human-readable cancellation policy text\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/booking-com/refs/heads/main/json-schema/booking-com-order-schema.json
tags: []
title: Booking.com Order
---
