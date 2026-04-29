---
description: ''
layout: schema
name: ExtraService
properties_list:
- description: extra service code, which can take following values code | name | - DSL | Driver language specified EWT | Extra waiting time MAG | Meet & Greet FLM | Flight monitoring NWS | Newspaper CAI | Cancellati
  name: code
  type: string
- description: extra service identifier
  name: itemId
  type: string
- description: extra service description
  name: description
  type: string
- description: extra service time metric type
  name: metricType
  type: string
- description: extra service metric value
  name: metricValue
  type: string
- description: ''
  name: quotation
  type: object
- description: ''
  name: converted
  type: object
- description: true if extra service is available for booking
  name: isBookable
  type: boolean
- description: true if tax included in extra service price
  name: taxIncluded
  type: boolean
- description: true if extra service price is included in total transfer amount
  name: includedInTotal
  type: boolean
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/transfer-search-extraservice-schema.json
slug: transfer-search-extraservice
source_filename: transfer-search-extraservice-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"ExtraService\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"extra service code, which can take following values\\n\\ncode   | name                                 \\n\\n | - \\n\\nDSL    | Driver language specified\\nEWT    | Extra waiting time\\nMAG    | Meet & Greet\\nFLM    | Flight monitoring\\nNWS    | Newspaper\\nCAI    | Cancellation insurance\\nWNR    | Wait and Return. Driver waits at destination and brings back the customer to pick-up point\\n\",\n      \"enum\": [\n        \"DSL\",\n        \"EWT\",\n        \"MAG\",\n        \"FLM\",\n        \"NWS\",\n        \"CAI\",\n        \"WNR\"\n      ]\n    },\n    \"itemId\": {\n      \"type\": \"string\",\n      \"description\": \"extra service identifier\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"extra service description\"\
  \n    },\n    \"metricType\": {\n      \"type\": \"string\",\n      \"description\": \"extra service time metric type\",\n      \"enum\": [\n        \"YEARS\",\n        \"DAYS\",\n        \"HOURS\",\n        \"MINUTES\"\n      ]\n    },\n    \"metricValue\": {\n      \"type\": \"string\",\n      \"description\": \"extra service metric value\"\n    },\n    \"quotation\": {\n      \"$ref\": \"#/definitions/Quotation\"\n    },\n    \"converted\": {\n      \"$ref\": \"#/definitions/Quotation\"\n    },\n    \"isBookable\": {\n      \"type\": \"boolean\",\n      \"description\": \"true if extra service is available for booking\"\n    },\n    \"taxIncluded\": {\n      \"type\": \"boolean\",\n      \"description\": \"true if tax included in extra service price\"\n    },\n    \"includedInTotal\": {\n      \"type\": \"boolean\",\n      \"description\": \"true if extra service price is included in total transfer amount\"\n    }\n  },\n  \"required\": [\n    \"code\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/transfer-search-extraservice-schema.json
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
title: ExtraService
---
