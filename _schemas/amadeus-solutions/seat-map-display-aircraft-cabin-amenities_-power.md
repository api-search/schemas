---
description: AircraftCabinAmenities_Power schema
layout: schema
name: AircraftCabinAmenities_Power
properties_list: []
provider_name: Amadeus Solutions
provider_slug: amadeus-solutions
schema_file: json-schema/seat-map-display-aircraft-cabin-amenities_-power-schema.json
slug: seat-map-display-aircraft-cabin-amenities_-power
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/seat-map-display-aircraft-cabin-amenities_-power-schema.json\",\n  \"title\": \"AircraftCabinAmenities_Power\",\n  \"description\": \"AircraftCabinAmenities_Power schema\",\n  \"allOf\": [\n    {\n      \"$ref\": \"#/definitions/Amenity\"\n    },\n    {\n      \"type\": \"object\",\n      \"description\": \"Type of power outlet for a given flight\",\n      \"properties\": {\n        \"powerType\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"PLUG\",\n            \"USB_PORT\",\n            \"ADAPTOR\",\n            \"PLUG_OR_USB_PORT\"\n          ]\n        },\n        \"usbType\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"USB_A\",\n            \"USB_C\",\n            \"USB_A_AND_USB_C\"\n          ]\n        }\n      }\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/seat-map-display-aircraft-cabin-amenities_-power-schema.json
tags:
- Airlines
- Booking
- Flights
- GDS
- Hotels
- Travel
- Travel Technology
title: AircraftCabinAmenities_Power
---
