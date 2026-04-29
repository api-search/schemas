---
description: ''
layout: schema
name: Vehicle
properties_list:
- description: vehicle type, which can take following values value | description -- | CAR | Car SED | Sedan WGN | Wagon ELC | Electric car VAN | Van or minivan SUV | Sport utility vehicle LMS | Limousine MBR | Motor
  name: code
  type: string
- description: category of the vehicle, which can take following values value | description -- | ST | Standard BU | Business FC | First class
  name: category
  type: string
- description: description of the vehicle. Can describe a list of potential vehicles, e.g. VW Polo or similar
  name: description
  type: string
- description: ''
  name: seats
  type: array
- description: ''
  name: baggages
  type: array
- description: URL to vehicle image
  name: imageURL
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/transfer-booking-vehicle-schema.json
slug: transfer-booking-vehicle
source_filename: transfer-booking-vehicle-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Vehicle\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"vehicle type, which can take following values\\n\\nvalue           | description\\n--  | \\nCAR             | Car\\nSED             | Sedan\\nWGN             | Wagon\\nELC             | Electric car\\nVAN             | Van or minivan\\nSUV             | Sport utility vehicle\\nLMS             | Limousine\\nMBR             | Motorbike\\nTRN             | Train\\nBUS             | Bus\\nHLC             | Helicopter (accessible only for private jet transfer)\\nJET             | Jet (accessible only for private jet transfer)\\n\",\n      \"enum\": [\n        \"CAR\",\n        \"SED\",\n        \"WGN\",\n        \"ELC\",\n        \"VAN\",\n        \"SUV\",\n        \"LMS\",\n        \"MBR\",\n        \"TRN\",\n        \"BUS\",\n        \"HLC\",\n        \"JET\"\n      ]\n  \
  \  },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"category of the vehicle, which can take following values\\n\\nvalue           | description\\n--  | \\nST              | Standard\\nBU              | Business\\nFC              | First class\\n\",\n      \"enum\": [\n        \"ST\",\n        \"BU\",\n        \"FC\"\n      ]\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"description of the vehicle. Can describe a list of potential vehicles, e.g. VW Polo or similar\"\n    },\n    \"seats\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/Seat\"\n      }\n    },\n    \"baggages\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/Baggage\"\n      }\n    },\n    \"imageURL\": {\n      \"type\": \"string\",\n      \"description\": \"URL to vehicle image\"\n    }\n  },\n  \"required\": [\n    \"code\",\n    \"category\",\n    \"description\",\n    \"\
  seats\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/transfer-booking-vehicle-schema.json
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
title: Vehicle
---
