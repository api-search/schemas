---
description: A complete place representation from the Places API (New)
layout: schema
name: Place
properties_list:
- description: The resource name of this place in the format places/{placeId}.
  name: name
  type: string
- description: The unique place ID
  name: id
  type: string
- description: A set of type tags for this place. Full list at https://developers.google.com/maps/documentation/places/web-service/place-types
  name: types
  type: array
- description: The primary type of this place
  name: primaryType
  type: string
- description: The place's phone number in national format
  name: nationalPhoneNumber
  type: string
- description: The place's phone number in international format
  name: internationalPhoneNumber
  type: string
- description: The full human-readable address for this place
  name: formattedAddress
  type: string
- description: A short human-readable address for this place
  name: shortFormattedAddress
  type: string
- description: The individual address components of the place
  name: addressComponents
  type: array
- description: The place's rating on a scale of 1.0 to 5.0
  name: rating
  type: number
- description: The total number of user ratings
  name: userRatingCount
  type: integer
- description: A URL to the place's page on Google Maps
  name: googleMapsUri
  type: string
- description: The place's website URL
  name: websiteUri
  type: string
- description: The price level of the place
  name: priceLevel
  type: string
- description: The business status of the place
  name: businessStatus
  type: string
- description: Number of minutes this place's current timezone is offset from UTC
  name: utcOffsetMinutes
  type: integer
- description: Up to 5 reviews for this place
  name: reviews
  type: array
- description: Photos associated with this place
  name: photos
  type: array
- description: The place's address in adr microformat
  name: adrFormatAddress
  type: string
- description: A URL for an SVG icon mask
  name: iconMaskBaseUri
  type: string
- description: Background color for the icon in hex format
  name: iconBackgroundColor
  type: string
- description: Whether the place supports dine-in
  name: dineIn
  type: boolean
- description: Whether the place supports takeout
  name: takeout
  type: boolean
- description: Whether the place supports delivery
  name: delivery
  type: boolean
- description: Whether the place supports curbside pickup
  name: curbsidePickup
  type: boolean
- description: Whether the place supports reservations
  name: reservable
  type: boolean
- description: ''
  name: servesBreakfast
  type: boolean
- description: ''
  name: servesLunch
  type: boolean
- description: ''
  name: servesDinner
  type: boolean
- description: ''
  name: servesBeer
  type: boolean
- description: ''
  name: servesWine
  type: boolean
- description: ''
  name: servesVegetarianFood
  type: boolean
provider_name: Google Maps Platform
provider_slug: google-maps
schema_file: json-schema/google-maps-places-place-schema.json
slug: google-maps-places-place
source_filename: google-maps-places-place-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Place\",\n  \"type\": \"object\",\n  \"description\": \"A complete place representation from the Places API (New)\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The resource name of this place in the format places/{placeId}.\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique place ID\"\n    },\n    \"types\": {\n      \"type\": \"array\",\n      \"description\": \"A set of type tags for this place. Full list at https://developers.google.com/maps/documentation/places/web-service/place-types\"\n    },\n    \"primaryType\": {\n      \"type\": \"string\",\n      \"description\": \"The primary type of this place\"\n    },\n    \"nationalPhoneNumber\": {\n      \"type\": \"string\",\n      \"description\": \"The place's phone number in national format\"\n    },\n    \"internationalPhoneNumber\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"The place's phone number in international format\"\n    },\n    \"formattedAddress\": {\n      \"type\": \"string\",\n      \"description\": \"The full human-readable address for this place\"\n    },\n    \"shortFormattedAddress\": {\n      \"type\": \"string\",\n      \"description\": \"A short human-readable address for this place\"\n    },\n    \"addressComponents\": {\n      \"type\": \"array\",\n      \"description\": \"The individual address components of the place\"\n    },\n    \"rating\": {\n      \"type\": \"number\",\n      \"description\": \"The place's rating on a scale of 1.0 to 5.0\"\n    },\n    \"userRatingCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The total number of user ratings\"\n    },\n    \"googleMapsUri\": {\n      \"type\": \"string\",\n      \"description\": \"A URL to the place's page on Google Maps\"\n    },\n    \"websiteUri\": {\n      \"type\": \"string\",\n      \"description\": \"The place's\
  \ website URL\"\n    },\n    \"priceLevel\": {\n      \"type\": \"string\",\n      \"description\": \"The price level of the place\"\n    },\n    \"businessStatus\": {\n      \"type\": \"string\",\n      \"description\": \"The business status of the place\"\n    },\n    \"utcOffsetMinutes\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of minutes this place's current timezone is offset from UTC\"\n    },\n    \"reviews\": {\n      \"type\": \"array\",\n      \"description\": \"Up to 5 reviews for this place\"\n    },\n    \"photos\": {\n      \"type\": \"array\",\n      \"description\": \"Photos associated with this place\"\n    },\n    \"adrFormatAddress\": {\n      \"type\": \"string\",\n      \"description\": \"The place's address in adr microformat\"\n    },\n    \"iconMaskBaseUri\": {\n      \"type\": \"string\",\n      \"description\": \"A URL for an SVG icon mask\"\n    },\n    \"iconBackgroundColor\": {\n      \"type\": \"string\",\n      \"description\": \"\
  Background color for the icon in hex format\"\n    },\n    \"dineIn\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the place supports dine-in\"\n    },\n    \"takeout\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the place supports takeout\"\n    },\n    \"delivery\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the place supports delivery\"\n    },\n    \"curbsidePickup\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the place supports curbside pickup\"\n    },\n    \"reservable\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the place supports reservations\"\n    },\n    \"servesBreakfast\": {\n      \"type\": \"boolean\"\n    },\n    \"servesLunch\": {\n      \"type\": \"boolean\"\n    },\n    \"servesDinner\": {\n      \"type\": \"boolean\"\n    },\n    \"servesBeer\": {\n      \"type\": \"boolean\"\n    },\n    \"servesWine\": {\n      \"type\": \"boolean\"\n    },\n    \"servesVegetarianFood\"\
  : {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-maps/refs/heads/main/json-schema/google-maps-places-place-schema.json
tags:
- Environment
- Geocoding
- Geolocation
- Maps
- Navigation
- Places
- Routing
- Solar
title: Place
---
