---
description: Phone information.
layout: schema
name: phone
properties_list:
- description: Category of the contact element
  name: category
  type: string
- description: Country code of the country (ISO3166-1). E.g. "US" for the United States
  name: countryCode
  type: string
- description: Phone number. Composed of digits only. The number of digits depends on the country.
  name: number
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/trip-parser-phone-schema.json
slug: trip-parser-phone
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"phone\",\n  \"description\": \"Phone information.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Category of the contact element\",\n      \"enum\": [\n        \"BUSINESS\",\n        \"PERSONAL\",\n        \"OTHER\"\n      ]\n    },\n    \"countryCode\": {\n      \"type\": \"string\",\n      \"description\": \"Country code of the country (ISO3166-1). E.g. \\\"US\\\" for the United States\"\n    },\n    \"number\": {\n      \"type\": \"string\",\n      \"description\": \"Phone number. Composed of digits only. The number of digits depends on the country.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/trip-parser-phone-schema.json
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
title: phone
---
