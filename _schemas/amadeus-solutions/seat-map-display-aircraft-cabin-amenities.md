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
provider_name: Amadeus Solutions
provider_slug: amadeus-solutions
schema_file: json-schema/seat-map-display-aircraft-cabin-amenities-schema.json
slug: seat-map-display-aircraft-cabin-amenities
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/seat-map-display-aircraft-cabin-amenities-schema.json\",\n  \"title\": \"AircraftCabinAmenities\",\n  \"description\": \"Type of available amenities for a given flight\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"power\": {\n      \"$ref\": \"#/definitions/AircraftCabinAmenities_Power\"\n    },\n    \"seat\": {\n      \"$ref\": \"#/definitions/Amenity_Seat\"\n    },\n    \"wifi\": {\n      \"$ref\": \"#/definitions/AircraftCabinAmenities_Wifi\"\n    },\n    \"entertainment\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/AircraftCabinAmenities_Entertainment\"\n      }\n    },\n    \"food\": {\n      \"$ref\": \"#/definitions/AircraftCabinAmenities_Food\"\n    },\n    \"beverage\": {\n      \"$ref\": \"#/definitions/AircraftCabinAmenities_Beverage\"\n\
  \    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/seat-map-display-aircraft-cabin-amenities-schema.json
tags:
- Airlines
- Booking
- Flights
- GDS
- Hotels
- Travel
- Travel Technology
title: AircraftCabinAmenities
---
