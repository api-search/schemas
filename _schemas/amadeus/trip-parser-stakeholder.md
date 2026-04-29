---
description: Definition of PNR travelers. Fields gender, nationality, placeOfBirth, countryOfResidence are only populated for passengerDelivery resources.
layout: schema
name: stakeholder
properties_list:
- description: item identifier
  name: id
  type: string
- description: Nationality of the Stakeholder
  name: nationality
  type: string
- description: '3-characters code defining the passenger type - possible values: ADT, CHD, INS, INF, UNA'
  name: passangerTypeCode
  type: string
- description: The individual's date of birth.
  name: dateOfBirth
  type: string
- description: Current age of the individual.
  name: age
  type: integer
- description: ''
  name: name
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/trip-parser-stakeholder-schema.json
slug: trip-parser-stakeholder
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"stakeholder\",\n  \"description\": \"Definition of PNR travelers. Fields gender, nationality, placeOfBirth, countryOfResidence are only populated for passengerDelivery resources.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"item identifier\"\n    },\n    \"nationality\": {\n      \"type\": \"string\",\n      \"description\": \"Nationality of the Stakeholder\"\n    },\n    \"passangerTypeCode\": {\n      \"type\": \"string\",\n      \"description\": \"3-characters code defining the passenger type - possible values: ADT, CHD, INS, INF, UNA\"\n    },\n    \"dateOfBirth\": {\n      \"type\": \"string\",\n      \"description\": \"The individual's date of birth.\"\n    },\n    \"age\": {\n      \"type\": \"integer\",\n      \"description\": \"Current age of the individual.\"\n    },\n    \"name\": {\n      \"$ref\": \"#/definitions/name\"\
  \n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/trip-parser-stakeholder-schema.json
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
title: stakeholder
---
