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
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://booking.com/schemas/booking-com/accommodation.json\",\n  \"title\": \"Booking.com Accommodation\",\n  \"description\": \"Represents an accommodation property listed on Booking.com, including hotels, apartments, hostels, and other lodging types with their details, facilities, and location information.\",\n  \"type\": \"object\",\n  \"required\": [\"accommodation_id\", \"name\", \"country\"],\n  \"properties\": {\n    \"accommodation_id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique numeric identifier for the accommodation on Booking.com\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the accommodation property\",\n      \"minLength\": 1,\n      \"maxLength\": 500\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Detailed text description of the accommodation and its offerings\"\n\
  \    },\n    \"address\": {\n      \"type\": \"string\",\n      \"description\": \"Street address of the accommodation\"\n    },\n    \"city\": {\n      \"type\": \"string\",\n      \"description\": \"City where the accommodation is located\"\n    },\n    \"city_id\": {\n      \"type\": \"integer\",\n      \"description\": \"Booking.com city identifier used for search queries\"\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"description\": \"Two-letter ISO 3166-1 alpha-2 country code\",\n      \"pattern\": \"^[A-Za-z]{2}$\"\n    },\n    \"zip\": {\n      \"type\": \"string\",\n      \"description\": \"Postal or ZIP code\"\n    },\n    \"location\": {\n      \"$ref\": \"#/$defs/GeoLocation\"\n    },\n    \"accommodation_type\": {\n      \"type\": \"integer\",\n      \"description\": \"Numeric identifier for the type of accommodation (hotel, apartment, hostel, etc.)\"\n    },\n    \"accommodation_type_name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable\
  \ name for the accommodation type\"\n    },\n    \"star_rating\": {\n      \"type\": \"number\",\n      \"description\": \"Official star rating classification of the property\",\n      \"minimum\": 0,\n      \"maximum\": 5\n    },\n    \"review_score\": {\n      \"type\": \"number\",\n      \"description\": \"Average guest review score on a scale of 1 to 10\",\n      \"minimum\": 1,\n      \"maximum\": 10\n    },\n    \"total_reviews\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of guest reviews for this accommodation\",\n      \"minimum\": 0\n    },\n    \"chain_id\": {\n      \"type\": \"integer\",\n      \"description\": \"Identifier for the hotel chain or brand, if applicable\"\n    },\n    \"chain_name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the hotel chain or brand, if applicable\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Default currency code for the property (ISO 4217)\",\n      \"\
  pattern\": \"^[A-Z]{3}$\"\n    },\n    \"checkin_from\": {\n      \"type\": \"string\",\n      \"description\": \"Earliest check-in time in HH:MM format\",\n      \"pattern\": \"^\\\\d{2}:\\\\d{2}$\"\n    },\n    \"checkin_until\": {\n      \"type\": \"string\",\n      \"description\": \"Latest check-in time in HH:MM format\",\n      \"pattern\": \"^\\\\d{2}:\\\\d{2}$\"\n    },\n    \"checkout_from\": {\n      \"type\": \"string\",\n      \"description\": \"Earliest checkout time in HH:MM format\",\n      \"pattern\": \"^\\\\d{2}:\\\\d{2}$\"\n    },\n    \"checkout_until\": {\n      \"type\": \"string\",\n      \"description\": \"Latest checkout time in HH:MM format\",\n      \"pattern\": \"^\\\\d{2}:\\\\d{2}$\"\n    },\n    \"facilities\": {\n      \"type\": \"array\",\n      \"description\": \"List of facilities and amenities available at the property\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Facility\"\n      }\n    },\n    \"photos\": {\n      \"type\": \"array\",\n     \
  \ \"description\": \"Photos of the accommodation property\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Photo\"\n      }\n    },\n    \"rooms\": {\n      \"type\": \"array\",\n      \"description\": \"Room types available at the accommodation\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Room\"\n      }\n    },\n    \"themes\": {\n      \"type\": \"array\",\n      \"description\": \"Thematic categories the accommodation belongs to\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"GeoLocation\": {\n      \"type\": \"object\",\n      \"description\": \"Geographic coordinates of a location\",\n      \"required\": [\"latitude\", \"longitude\"],\n      \"properties\": {\n        \"latitude\": {\n          \"type\": \"number\",\n          \"description\": \"Latitude coordinate in decimal degrees\",\n          \"minimum\": -90,\n          \"maximum\": 90\n        },\n        \"longitude\": {\n          \"type\": \"number\",\n       \
  \   \"description\": \"Longitude coordinate in decimal degrees\",\n          \"minimum\": -180,\n          \"maximum\": 180\n        }\n      }\n    },\n    \"Facility\": {\n      \"type\": \"object\",\n      \"description\": \"A facility or amenity available at the property or room level\",\n      \"required\": [\"facility_id\", \"name\"],\n      \"properties\": {\n        \"facility_id\": {\n          \"type\": \"integer\",\n          \"description\": \"Unique facility identifier\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Human-readable facility name\"\n        },\n        \"facility_type\": {\n          \"type\": \"string\",\n          \"description\": \"Category of the facility\"\n        }\n      }\n    },\n    \"Photo\": {\n      \"type\": \"object\",\n      \"description\": \"A photo of the accommodation or its rooms\",\n      \"required\": [\"url\"],\n      \"properties\": {\n        \"photo_id\": {\n          \"type\": \"\
  string\",\n          \"description\": \"Unique photo identifier\"\n        },\n        \"url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL where the photo can be accessed\"\n        },\n        \"tag\": {\n          \"type\": \"string\",\n          \"description\": \"Category tag for the photo (e.g., room, exterior, lobby)\"\n        },\n        \"sort_order\": {\n          \"type\": \"integer\",\n          \"description\": \"Display sort order for the photo\"\n        }\n      }\n    },\n    \"Room\": {\n      \"type\": \"object\",\n      \"description\": \"A room type available at the accommodation\",\n      \"required\": [\"room_id\", \"name\"],\n      \"properties\": {\n        \"room_id\": {\n          \"type\": \"integer\",\n          \"description\": \"Unique room type identifier\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Room type name\"\n        },\n        \"max_occupancy\"\
  : {\n          \"type\": \"integer\",\n          \"description\": \"Maximum number of guests the room can accommodate\",\n          \"minimum\": 1\n        },\n        \"room_size\": {\n          \"type\": \"number\",\n          \"description\": \"Room size in square meters\"\n        },\n        \"bed_configurations\": {\n          \"type\": \"array\",\n          \"description\": \"Available bed configurations for this room type\",\n          \"items\": {\n            \"$ref\": \"#/$defs/BedConfiguration\"\n          }\n        },\n        \"facilities\": {\n          \"type\": \"array\",\n          \"description\": \"Room-level facilities and amenities\",\n          \"items\": {\n            \"$ref\": \"#/$defs/Facility\"\n          }\n        }\n      }\n    },\n    \"BedConfiguration\": {\n      \"type\": \"object\",\n      \"description\": \"A bed configuration option for a room\",\n      \"properties\": {\n        \"bed_type\": {\n          \"type\": \"string\",\n          \"description\"\
  : \"Type of bed (e.g., double, twin, king, queen)\"\n        },\n        \"bed_type_id\": {\n          \"type\": \"integer\",\n          \"description\": \"Numeric bed type identifier\"\n        },\n        \"quantity\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of beds of this type\",\n          \"minimum\": 1\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/booking-com/refs/heads/main/json-schema/booking-com-accommodation-schema.json
tags: []
title: Booking.com Accommodation
---
