---
description: AircraftCabinAmenities_Beverage schema
layout: schema
name: AircraftCabinAmenities_Beverage
properties_list: []
provider_name: Amadeus Solutions
provider_slug: amadeus-solutions
schema_file: json-schema/seat-map-display-aircraft-cabin-amenities_-beverage-schema.json
slug: seat-map-display-aircraft-cabin-amenities_-beverage
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/seat-map-display-aircraft-cabin-amenities_-beverage-schema.json\",\n  \"title\": \"AircraftCabinAmenities_Beverage\",\n  \"description\": \"AircraftCabinAmenities_Beverage schema\",\n  \"allOf\": [\n    {\n      \"$ref\": \"#/definitions/Amenity\"\n    },\n    {\n      \"type\": \"object\",\n      \"description\": \"Type of beverage for a given flight\",\n      \"properties\": {\n        \"beverageType\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"ALCOHOLIC\",\n            \"NON_ALCOHOLIC\",\n            \"ALCOHOLIC_AND_NON_ALCOHOLIC\"\n          ]\n        }\n      }\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/seat-map-display-aircraft-cabin-amenities_-beverage-schema.json
tags:
- Airlines
- Booking
- Flights
- GDS
- Hotels
- Travel
- Travel Technology
title: AircraftCabinAmenities_Beverage
---
