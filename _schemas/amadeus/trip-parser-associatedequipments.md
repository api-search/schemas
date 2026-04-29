---
description: Used to convey information about special equipments (GPS, Baby seat, ...) associated to the car booking.
layout: schema
name: associatedEquipments
properties_list:
- description: Equipment name
  name: name
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/trip-parser-associatedequipments-schema.json
slug: trip-parser-associatedequipments
source_filename: trip-parser-associatedequipments-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"associatedEquipments\",\n  \"description\": \"Used to convey information about special equipments (GPS, Baby seat, ...) associated to the car booking.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Equipment name\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/trip-parser-associatedequipments-schema.json
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
title: associatedEquipments
---
