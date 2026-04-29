---
description: 'seat characteristics dictionary allows mapping a service characteristic to its name. Possible values are part of: IATA code: Most of the codes are defined by IATA Standard/IATA Code list 9825, Example: CH = Chargeable Seat, W = Window Seat, A = Aisle Seat, Q = Seat in a quiet zone, E = Exit Row Seat Amadeus Code: defined as extension, example MV=row with movie screen Seat map display Code: API specific codes, example 1A_AQC_PREMIUM_SEAT=premium seat'
layout: schema
name: SeatCharacteristicDictionary
properties_list: []
provider_name: Amadeus Solutions
provider_slug: amadeus-solutions
schema_file: json-schema/seat-map-display-seat-characteristic-dictionary-schema.json
slug: seat-map-display-seat-characteristic-dictionary
source_filename: seat-map-display-seat-characteristic-dictionary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/seat-map-display-seat-characteristic-dictionary-schema.json\",\n  \"title\": \"SeatCharacteristicDictionary\",\n  \"description\": \"seat characteristics dictionary allows mapping a service characteristic to its name. Possible values are part of:\\n  IATA code: Most of the codes are defined by IATA Standard/IATA Code list 9825, Example: CH = Chargeable Seat, W = Window Seat, A = Aisle\\n             Seat, Q = Seat in a quiet zone, E = Exit Row Seat\\n  Amadeus Code: defined as extension, example MV=row with movie screen\\n  Seat map display Code: API specific codes, example 1A_AQC_PREMIUM_SEAT=premium seat\",\n  \"type\": \"object\",\n  \"additionalProperties\": {\n    \"type\": \"string\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/seat-map-display-seat-characteristic-dictionary-schema.json
tags:
- Airlines
- Booking
- Flights
- GDS
- Hotels
- Travel
- Travel Technology
title: SeatCharacteristicDictionary
---
