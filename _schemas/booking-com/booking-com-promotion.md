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
tags: []
title: Booking.com Promotion
---
