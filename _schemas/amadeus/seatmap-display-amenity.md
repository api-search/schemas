---
description: 'Base data model related to Amenity, inherited amenities can be created using this baseline for extension ( using type for polymorphism ) amenityType : Enum related to generic Amenity model to identify which amenityType'
layout: schema
name: Amenity
properties_list:
- description: Specify if the traveler will need to pay extra in-flight to get the amenity
  name: isChargeable
  type: boolean
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/seatmap-display-amenity-schema.json
slug: seatmap-display-amenity
source_filename: seatmap-display-amenity-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Amenity\",\n  \"description\": \"Base data model related to Amenity, inherited amenities can be created using this baseline for extension ( using type for polymorphism ) amenityType : Enum related to generic Amenity model to identify which amenityType\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"isChargeable\": {\n      \"type\": \"boolean\",\n      \"description\": \"Specify if the traveler will need to pay extra in-flight to get the amenity\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/seatmap-display-amenity-schema.json
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
title: Amenity
---
