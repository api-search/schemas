---
description: 'Base data model related to Amenity, inherited amenities can be created using this baseline for extension ( using type for polymorphism ) amenityType : Enum related to generic Amenity model to identify which amenityType'
layout: schema
name: Amenity
properties_list:
- description: Specify if the traveler will need to pay extra in-flight to get the amenity
  name: isChargeable
  type: boolean
provider_name: Amadeus Solutions
provider_slug: amadeus-solutions
schema_file: json-schema/seat-map-display-amenity-schema.json
slug: seat-map-display-amenity
source_filename: seat-map-display-amenity-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/seat-map-display-amenity-schema.json\",\n  \"title\": \"Amenity\",\n  \"description\": \"Base data model related to Amenity, inherited amenities can be created using this baseline for extension ( using type for polymorphism ) amenityType : Enum related to generic Amenity model to identify which amenityType\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"isChargeable\": {\n      \"description\": \"Specify if the traveler will need to pay extra in-flight to get the amenity\",\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/seat-map-display-amenity-schema.json
tags:
- Airlines
- Booking
- Flights
- GDS
- Hotels
- Travel
- Travel Technology
title: Amenity
---
