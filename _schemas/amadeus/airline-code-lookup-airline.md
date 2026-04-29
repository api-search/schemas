---
description: An airline resource containing identifying codes and names for a single airline carrier.
layout: schema
name: Airline
properties_list:
- description: Resource type identifier.
  name: type
  type: string
- description: Two-letter IATA airline designator code.
  name: iataCode
  type: string
- description: Three-letter ICAO airline designator code.
  name: icaoCode
  type: string
- description: The official business name of the airline.
  name: businessName
  type: string
- description: The commonly used abbreviated name of the airline.
  name: commonName
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/airline-code-lookup-airline-schema.json
slug: airline-code-lookup-airline
source_filename: airline-code-lookup-airline-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Airline\",\n  \"description\": \"An airline resource containing identifying codes and names for a single airline carrier.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Resource type identifier.\"\n    },\n    \"iataCode\": {\n      \"type\": \"string\",\n      \"description\": \"Two-letter IATA airline designator code.\"\n    },\n    \"icaoCode\": {\n      \"type\": \"string\",\n      \"description\": \"Three-letter ICAO airline designator code.\"\n    },\n    \"businessName\": {\n      \"type\": \"string\",\n      \"description\": \"The official business name of the airline.\"\n    },\n    \"commonName\": {\n      \"type\": \"string\",\n      \"description\": \"The commonly used abbreviated name of the airline.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/airline-code-lookup-airline-schema.json
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
title: Airline
---
