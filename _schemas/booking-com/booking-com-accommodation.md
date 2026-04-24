---
description: Represents an accommodation property listed on Booking.com, including hotels, apartments, hostels, and other lodging types with their details, facilities, and location information.
layout: schema
name: Booking.com Accommodation
properties_list:
- description: Unique numeric identifier for the accommodation on Booking.com
  name: accommodation_id
  type: integer
- description: Display name of the accommodation property
  name: name
  type: string
- description: Detailed text description of the accommodation and its offerings
  name: description
  type: string
- description: Street address of the accommodation
  name: address
  type: string
- description: City where the accommodation is located
  name: city
  type: string
- description: Booking.com city identifier used for search queries
  name: city_id
  type: integer
- description: Two-letter ISO 3166-1 alpha-2 country code
  name: country
  type: string
- description: Postal or ZIP code
  name: zip
  type: string
- description: ''
  name: location
  type: object
- description: Numeric identifier for the type of accommodation (hotel, apartment, hostel, etc.)
  name: accommodation_type
  type: integer
- description: Human-readable name for the accommodation type
  name: accommodation_type_name
  type: string
- description: Official star rating classification of the property
  name: star_rating
  type: number
- description: Average guest review score on a scale of 1 to 10
  name: review_score
  type: number
- description: Total number of guest reviews for this accommodation
  name: total_reviews
  type: integer
- description: Identifier for the hotel chain or brand, if applicable
  name: chain_id
  type: integer
- description: Name of the hotel chain or brand, if applicable
  name: chain_name
  type: string
- description: Default currency code for the property (ISO 4217)
  name: currency
  type: string
- description: Earliest check-in time in HH:MM format
  name: checkin_from
  type: string
- description: Latest check-in time in HH:MM format
  name: checkin_until
  type: string
- description: Earliest checkout time in HH:MM format
  name: checkout_from
  type: string
- description: Latest checkout time in HH:MM format
  name: checkout_until
  type: string
- description: List of facilities and amenities available at the property
  name: facilities
  type: array
- description: Photos of the accommodation property
  name: photos
  type: array
- description: Room types available at the accommodation
  name: rooms
  type: array
- description: Thematic categories the accommodation belongs to
  name: themes
  type: array
provider_name: booking-com
provider_slug: booking-com
schema_file: json-schema/booking-com-accommodation-schema.json
slug: booking-com-accommodation
tags: []
title: Booking.com Accommodation
---
