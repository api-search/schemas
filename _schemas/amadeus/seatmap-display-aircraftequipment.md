---
description: information related to the aircraft
layout: schema
name: AircraftEquipment
properties_list:
- description: IATA aircraft code (http://www.flugzeuginfo.net/table_accodes_iata_en.php)
  name: code
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/seatmap-display-aircraftequipment-schema.json
slug: seatmap-display-aircraftequipment
source_filename: seatmap-display-aircraftequipment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"AircraftEquipment\",\n  \"description\": \"information related to the aircraft\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"IATA aircraft code (http://www.flugzeuginfo.net/table_accodes_iata_en.php)\\n\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/seatmap-display-aircraftequipment-schema.json
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
title: AircraftEquipment
---
