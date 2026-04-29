---
description: information related to the aircraft
layout: schema
name: AircraftEquipment
properties_list:
- description: IATA aircraft code (http://www.flugzeuginfo.net/table_accodes_iata_en.php)
  name: code
  type: string
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/flight-order-management-aircraft-equipment-schema.json
slug: flight-order-management-aircraft-equipment
source_filename: flight-order-management-aircraft-equipment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-order-management-aircraft-equipment-schema.json\",\n  \"title\": \"AircraftEquipment\",\n  \"description\": \"information related to the aircraft\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"IATA aircraft code (http://www.flugzeuginfo.net/table_accodes_iata_en.php)\\n\",\n      \"pattern\": \"[a-zA-Z0-9]{3}\",\n      \"example\": \"318\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-order-management-aircraft-equipment-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: AircraftEquipment
---
