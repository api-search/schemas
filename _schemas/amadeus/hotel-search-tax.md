---
description: 'IATA Tax definition: An impost for raising revenue for the general treasury and which will be used for general public purposes.'
layout: schema
name: Tax
properties_list:
- description: Defines amount with decimal separator.
  name: amount
  type: string
- description: 'Defines a monetary unit. It is a three alpha code (iata code). Example: EUR for Euros, USD for US dollar, etc.'
  name: currency
  type: string
- description: International Standards Organization (ISO) Tax code.It is a two-letter country code.
  name: code
  type: string
- description: In the case of a tax on TST value, the percentage of the tax will be indicated in this field.
  name: percentage
  type: string
- description: Indicates if tax is included or not
  name: included
  type: boolean
- description: Example - "Governement tax"
  name: description
  type: string
- description: Specifies if the tax applies per stay or per night - PER_STAY - PER_NIGHT
  name: pricingFrequency
  type: string
- description: Specifies if the tax applies per occupant or per room - PER_OCCUPANT - PER_PRODUCT
  name: pricingMode
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/hotel-search-tax-schema.json
slug: hotel-search-tax
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Tax\",\n  \"description\": \"IATA Tax definition: An impost for raising revenue for the general treasury and which will be used for general public purposes.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"amount\": {\n      \"type\": \"string\",\n      \"description\": \"Defines amount with decimal separator.\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Defines a monetary unit. It is a three alpha code (iata code). Example: EUR for Euros, USD for US dollar, etc.\"\n    },\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"International Standards Organization (ISO) Tax code.It is a two-letter country code.\"\n    },\n    \"percentage\": {\n      \"type\": \"string\",\n      \"description\": \"In the case of a tax on TST value, the percentage of the tax will be indicated in this field.\"\n    },\n    \"included\": {\n      \"type\"\
  : \"boolean\",\n      \"description\": \"Indicates if tax is included or not\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Example - \\\"Governement tax\\\"\"\n    },\n    \"pricingFrequency\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies if the tax applies per stay or per night\\n  - PER_STAY\\n  - PER_NIGHT\"\n    },\n    \"pricingMode\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies if the tax applies per occupant or per room\\n  - PER_OCCUPANT\\n  - PER_PRODUCT\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/hotel-search-tax-schema.json
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
title: Tax
---
