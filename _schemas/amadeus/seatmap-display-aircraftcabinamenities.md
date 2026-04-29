---
description: Type of available amenities for a given flight
layout: schema
name: AircraftCabinAmenities
properties_list:
- description: ''
  name: power
  type: object
- description: ''
  name: seat
  type: object
- description: ''
  name: wifi
  type: object
- description: ''
  name: entertainment
  type: array
- description: ''
  name: food
  type: object
- description: ''
  name: beverage
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/seatmap-display-aircraftcabinamenities-schema.json
slug: seatmap-display-aircraftcabinamenities
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"AircraftCabinAmenities\",\n  \"description\": \"Type of available amenities for a given flight\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"power\": {\n      \"$ref\": \"#/definitions/AircraftCabinAmenities_Power\"\n    },\n    \"seat\": {\n      \"$ref\": \"#/definitions/Amenity_Seat\"\n    },\n    \"wifi\": {\n      \"$ref\": \"#/definitions/AircraftCabinAmenities_Wifi\"\n    },\n    \"entertainment\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/AircraftCabinAmenities_Entertainment\"\n      }\n    },\n    \"food\": {\n      \"$ref\": \"#/definitions/AircraftCabinAmenities_Food\"\n    },\n    \"beverage\": {\n      \"$ref\": \"#/definitions/AircraftCabinAmenities_Beverage\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/seatmap-display-aircraftcabinamenities-schema.json
tags:
- Airlines
- Aviation
- Booking
- Destinations
- Flights
- Hospitality
- Hotels
- Market Insights
- Tourism
- Transfers
- Travel
title: AircraftCabinAmenities
---
