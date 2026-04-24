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
tags: []
title: Booking.com Order
---
