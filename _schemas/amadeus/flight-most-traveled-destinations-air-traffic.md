---
description: ''
layout: schema
name: Air_Traffic
properties_list:
- description: ''
  name: type
  type: string
- description: ''
  name: subType
  type: string
- description: IATA code of the destination city - [IATA table codes](http://www.iata.org/publications/Pages/code-search.aspx)
  name: destination
  type: string
- description: ''
  name: analytics
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-most-traveled-destinations-air-traffic-schema.json
slug: flight-most-traveled-destinations-air-traffic
source_filename: flight-most-traveled-destinations-air-traffic-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Air_Traffic\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"subType\": {\n      \"type\": \"string\"\n    },\n    \"destination\": {\n      \"type\": \"string\",\n      \"description\": \"IATA code of the destination city - [IATA table codes](http://www.iata.org/publications/Pages/code-search.aspx)\"\n    },\n    \"analytics\": {\n      \"$ref\": \"#/definitions/Analytics\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/flight-most-traveled-destinations-air-traffic-schema.json
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
title: Air_Traffic
---
