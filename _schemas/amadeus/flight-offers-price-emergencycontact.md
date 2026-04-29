---
description: emergency contact number
layout: schema
name: EmergencyContact
properties_list:
- description: Adressee name (e.g. in case of emergency purpose it corresponds to name of the person to be contacted).
  name: addresseeName
  type: string
- description: Country code of the country (ISO3166-1). E.g. "US" for the United States
  name: countryCode
  type: string
- description: Phone number. Composed of digits only. The number of digits depends on the country.
  name: number
  type: string
- description: additional details
  name: text
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-offers-price-emergencycontact-schema.json
slug: flight-offers-price-emergencycontact
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"EmergencyContact\",\n  \"description\": \"emergency contact number\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"addresseeName\": {\n      \"type\": \"string\",\n      \"description\": \"Adressee name (e.g. in case of emergency purpose it corresponds to name of the person to be contacted).\"\n    },\n    \"countryCode\": {\n      \"type\": \"string\",\n      \"description\": \"Country code of the country (ISO3166-1). E.g. \\\"US\\\" for the United States\"\n    },\n    \"number\": {\n      \"type\": \"string\",\n      \"description\": \"Phone number. Composed of digits only. The number of digits depends on the country.\"\n    },\n    \"text\": {\n      \"type\": \"string\",\n      \"description\": \"additional details\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/flight-offers-price-emergencycontact-schema.json
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
title: EmergencyContact
---
