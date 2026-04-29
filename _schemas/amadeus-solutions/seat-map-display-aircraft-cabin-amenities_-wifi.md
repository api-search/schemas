---
description: AircraftCabinAmenities_Wifi schema
layout: schema
name: AircraftCabinAmenities_Wifi
properties_list: []
provider_name: Amadeus Solutions
provider_slug: amadeus-solutions
schema_file: json-schema/seat-map-display-aircraft-cabin-amenities_-wifi-schema.json
slug: seat-map-display-aircraft-cabin-amenities_-wifi
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/seat-map-display-aircraft-cabin-amenities_-wifi-schema.json\",\n  \"title\": \"AircraftCabinAmenities_Wifi\",\n  \"description\": \"AircraftCabinAmenities_Wifi schema\",\n  \"allOf\": [\n    {\n      \"$ref\": \"#/definitions/Amenity\"\n    },\n    {\n      \"type\": \"object\",\n      \"description\": \"Level of area coverage for a given flight\",\n      \"properties\": {\n        \"wifiCoverage\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"FULL\",\n            \"PARTIAL\"\n          ]\n        }\n      }\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/seat-map-display-aircraft-cabin-amenities_-wifi-schema.json
tags:
- Airlines
- Booking
- Flights
- GDS
- Hotels
- Travel
- Travel Technology
title: AircraftCabinAmenities_Wifi
---
