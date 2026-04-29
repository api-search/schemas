---
description: AircraftCabinAmenities_Food schema
layout: schema
name: AircraftCabinAmenities_Food
properties_list: []
provider_name: Amadeus Solutions
provider_slug: amadeus-solutions
schema_file: json-schema/seat-map-display-aircraft-cabin-amenities_-food-schema.json
slug: seat-map-display-aircraft-cabin-amenities_-food
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/seat-map-display-aircraft-cabin-amenities_-food-schema.json\",\n  \"title\": \"AircraftCabinAmenities_Food\",\n  \"description\": \"AircraftCabinAmenities_Food schema\",\n  \"allOf\": [\n    {\n      \"$ref\": \"#/definitions/Amenity\"\n    },\n    {\n      \"type\": \"object\",\n      \"description\": \"Type of food for a given flight\",\n      \"properties\": {\n        \"foodType\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"MEAL\",\n            \"FRESH_MEAL\",\n            \"SNACK\",\n            \"FRESH_SNACK\"\n          ]\n        }\n      }\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/seat-map-display-aircraft-cabin-amenities_-food-schema.json
tags:
- Airlines
- Booking
- Flights
- GDS
- Hotels
- Travel
- Travel Technology
title: AircraftCabinAmenities_Food
---
