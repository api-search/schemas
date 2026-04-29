---
description: Represents a promotional offer on Booking.com, including deals, discounts, and special rates that properties use to attract travelers and increase bookings.
layout: schema
name: Booking.com Promotion
properties_list:
- description: Unique identifier for the promotion
  name: promotion_id
  type: string
- description: Type of promotional offer
  name: promotion_type
  type: string
- description: Booking.com property identifier this promotion applies to
  name: hotel_id
  type: integer
- description: Discount percentage applied to the parent rate
  name: discount_percentage
  type: number
- description: Current status of the promotion
  name: status
  type: string
- description: Start date from which the promotion can be booked
  name: bookable_from
  type: string
- description: End date until which the promotion can be booked
  name: bookable_until
  type: string
- description: Earliest check-in date for stays using this promotion
  name: stay_from
  type: string
- description: Latest check-out date for stays using this promotion
  name: stay_until
  type: string
- description: Minimum number of days in advance the booking must be made
  name: min_advance_days
  type: integer
- description: Maximum number of days in advance the booking can be made
  name: max_advance_days
  type: integer
- description: Minimum number of nights required for the stay
  name: min_stay_nights
  type: integer
- description: Room type IDs this promotion applies to; empty means all rooms
  name: applicable_rooms
  type: array
- description: Rate plan IDs this promotion applies to; empty means all rates
  name: applicable_rates
  type: array
- description: Country codes eligible for this promotion (country_rate type only)
  name: target_countries
  type: array
- description: Device types eligible for this promotion (mobile_rate type only)
  name: target_devices
  type: array
- description: Name of the campaign (campaign_deal type only)
  name: campaign_name
  type: string
- description: Timestamp when the promotion was created
  name: created_at
  type: string
- description: Timestamp when the promotion was last modified
  name: modified_at
  type: string
provider_name: booking-com
provider_slug: booking-com
schema_file: json-schema/booking-com-promotion-schema.json
slug: booking-com-promotion
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://booking.com/schemas/booking-com/promotion.json\",\n  \"title\": \"Booking.com Promotion\",\n  \"description\": \"Represents a promotional offer on Booking.com, including deals, discounts, and special rates that properties use to attract travelers and increase bookings.\",\n  \"type\": \"object\",\n  \"required\": [\"promotion_id\", \"promotion_type\", \"discount_percentage\"],\n  \"properties\": {\n    \"promotion_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the promotion\"\n    },\n    \"promotion_type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of promotional offer\",\n      \"enum\": [\"basic_deal\", \"last_minute_deal\", \"campaign_deal\", \"country_rate\", \"mobile_rate\"]\n    },\n    \"hotel_id\": {\n      \"type\": \"integer\",\n      \"description\": \"Booking.com property identifier this promotion applies to\"\n   \
  \ },\n    \"discount_percentage\": {\n      \"type\": \"number\",\n      \"description\": \"Discount percentage applied to the parent rate\",\n      \"minimum\": 0,\n      \"maximum\": 100\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current status of the promotion\",\n      \"enum\": [\"active\", \"inactive\", \"expired\", \"pending\"]\n    },\n    \"bookable_from\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Start date from which the promotion can be booked\"\n    },\n    \"bookable_until\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"End date until which the promotion can be booked\"\n    },\n    \"stay_from\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Earliest check-in date for stays using this promotion\"\n    },\n    \"stay_until\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"\
  Latest check-out date for stays using this promotion\"\n    },\n    \"min_advance_days\": {\n      \"type\": \"integer\",\n      \"description\": \"Minimum number of days in advance the booking must be made\",\n      \"minimum\": 0\n    },\n    \"max_advance_days\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of days in advance the booking can be made\"\n    },\n    \"min_stay_nights\": {\n      \"type\": \"integer\",\n      \"description\": \"Minimum number of nights required for the stay\",\n      \"minimum\": 1\n    },\n    \"applicable_rooms\": {\n      \"type\": \"array\",\n      \"description\": \"Room type IDs this promotion applies to; empty means all rooms\",\n      \"items\": {\n        \"type\": \"integer\"\n      }\n    },\n    \"applicable_rates\": {\n      \"type\": \"array\",\n      \"description\": \"Rate plan IDs this promotion applies to; empty means all rates\",\n      \"items\": {\n        \"type\": \"integer\"\n      }\n    },\n    \"target_countries\"\
  : {\n      \"type\": \"array\",\n      \"description\": \"Country codes eligible for this promotion (country_rate type only)\",\n      \"items\": {\n        \"type\": \"string\",\n        \"pattern\": \"^[A-Za-z]{2}$\"\n      }\n    },\n    \"target_devices\": {\n      \"type\": \"array\",\n      \"description\": \"Device types eligible for this promotion (mobile_rate type only)\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\"mobile\", \"tablet\"]\n      }\n    },\n    \"campaign_name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the campaign (campaign_deal type only)\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the promotion was created\"\n    },\n    \"modified_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the promotion was last modified\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/booking-com/refs/heads/main/json-schema/booking-com-promotion-schema.json
tags: []
title: Booking.com Promotion
---
