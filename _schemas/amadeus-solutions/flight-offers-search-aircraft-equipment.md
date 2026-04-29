---
description: information related to the aircraft
layout: schema
name: AircraftEquipment
properties_list:
- description: IATA aircraft code (http://www.flugzeuginfo.net/table_accodes_iata_en.php)
  name: code
  type: string
provider_name: Amadeus Solutions
provider_slug: amadeus-solutions
schema_file: json-schema/flight-offers-search-aircraft-equipment-schema.json
slug: flight-offers-search-aircraft-equipment
source_filename: flight-offers-search-aircraft-equipment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/flight-offers-search-aircraft-equipment-schema.json\",\n  \"title\": \"AircraftEquipment\",\n  \"description\": \"information related to the aircraft\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"IATA aircraft code (http://www.flugzeuginfo.net/table_accodes_iata_en.php)\\n\",\n      \"pattern\": \"[a-zA-Z0-9]{3}\",\n      \"example\": \"318\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/flight-offers-search-aircraft-equipment-schema.json
tags:
- Airlines
- Booking
- Flights
- GDS
- Hotels
- Travel
- Travel Technology
title: AircraftEquipment
---
