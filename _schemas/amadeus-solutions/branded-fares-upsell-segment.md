---
description: Segment schema
layout: schema
name: Segment
properties_list: []
provider_name: Amadeus Solutions
provider_slug: amadeus-solutions
schema_file: json-schema/branded-fares-upsell-segment-schema.json
slug: branded-fares-upsell-segment
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/branded-fares-upsell-segment-schema.json\",\n  \"title\": \"Segment\",\n  \"description\": \"Segment schema\",\n  \"allOf\": [\n    {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"description\": \"Id of the segment\",\n          \"type\": \"string\",\n          \"example\": 1\n        },\n        \"numberOfStops\": {\n          \"description\": \"Number of stops\",\n          \"type\": \"integer\",\n          \"example\": 0\n        },\n        \"blacklistedInEU\": {\n          \"description\": \"When the flight has a marketing or/and operating airline that is identified as blacklisted by the European Commission. \\n\\nTo improve travel safety, the European Commission regularly updates the list of the banned carriers from operating in Europe. It allows any Travel\
  \ Agency located in the European Union to easily identify and hide any travel recommendation based on some unsafe airlines. \\nThe [list of the banned airlines](https://ec.europa.eu/transport/sites/transport/files/air-safety-list_en.pdf) is published in the Official Journal of the European Union, where they are included as annexes A and B to the Commission Regulation. The blacklist of an airline can concern all its flights or some specific aircraft types pertaining to the airline   \\n\",\n          \"type\": \"boolean\",\n          \"example\": false\n        },\n        \"co2Emissions\": {\n          \"description\": \"Co2 informations\",\n          \"type\": \"array\",\n          \"minItems\": 1,\n          \"items\": {\n            \"title\": \"Co2Emission\",\n            \"$ref\": \"#/definitions/Co2Emission\"\n          }\n        }\n      }\n    },\n    {\n      \"$ref\": \"#/definitions/FlightSegment\"\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/branded-fares-upsell-segment-schema.json
tags:
- Airlines
- Booking
- Flights
- GDS
- Hotels
- Travel
- Travel Technology
title: Segment
---
