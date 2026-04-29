---
description: Car Product
layout: schema
name: carData
properties_list:
- description: Confirmation number
  name: confirmationNumber
  type: string
- description: car provider information(Car rental compay name)
  name: serviceProviderName
  type: string
- description: ''
  name: associatedEquipments
  type: array
- description: ''
  name: pickup
  type: object
- description: ''
  name: dropoff
  type: object
- description: ''
  name: driver
  type: object
- description: ''
  name: vehicle
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/trip-parser-cardata-schema.json
slug: trip-parser-cardata
source_filename: trip-parser-cardata-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"carData\",\n  \"description\": \"Car Product\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"confirmationNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Confirmation number\"\n    },\n    \"serviceProviderName\": {\n      \"type\": \"string\",\n      \"description\": \"car provider information(Car rental compay name)\"\n    },\n    \"associatedEquipments\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/associatedEquipments\"\n      }\n    },\n    \"pickup\": {\n      \"$ref\": \"#/definitions/pickup\"\n    },\n    \"dropoff\": {\n      \"$ref\": \"#/definitions/dropoff\"\n    },\n    \"driver\": {\n      \"$ref\": \"#/definitions/driver\"\n    },\n    \"vehicle\": {\n      \"$ref\": \"#/definitions/carVehicle\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/trip-parser-cardata-schema.json
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
title: carData
---
