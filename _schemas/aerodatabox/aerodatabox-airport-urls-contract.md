---
description: Airport URLs contract
layout: schema
name: AirportUrlsContract
properties_list:
- description: Main web-site of the airport
  name: webSite
  type: string
- description: Wikipedia page of the airport
  name: wikipedia
  type: string
- description: Twitter feed of the airport
  name: twitter
  type: string
- description: LiveAtc page of the airport
  name: liveAtc
  type: string
- description: FlightRadar page of the airport
  name: flightRadar
  type: string
- description: Google Maps URL of the airport
  name: googleMaps
  type: string
provider_name: AeroDataBox
provider_slug: aerodatabox
schema_file: json-schema/aerodatabox-airport-urls-contract-schema.json
slug: aerodatabox-airport-urls-contract
source_filename: aerodatabox-airport-urls-contract-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-airport-urls-contract-schema.json\",\n  \"title\": \"AirportUrlsContract\",\n  \"description\": \"Airport URLs contract\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"webSite\": {\n      \"type\": \"string\",\n      \"description\": \"Main web-site of the airport\",\n      \"nullable\": true\n    },\n    \"wikipedia\": {\n      \"type\": \"string\",\n      \"description\": \"Wikipedia page of the airport\",\n      \"nullable\": true\n    },\n    \"twitter\": {\n      \"type\": \"string\",\n      \"description\": \"Twitter feed of the airport\",\n      \"nullable\": true\n    },\n    \"liveAtc\": {\n      \"type\": \"string\",\n      \"description\": \"LiveAtc page of the airport\",\n      \"nullable\": true\n    },\n    \"flightRadar\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"FlightRadar page of the airport\",\n      \"nullable\": true\n    },\n    \"googleMaps\": {\n      \"type\": \"string\",\n      \"description\": \"Google Maps URL of the airport\",\n      \"nullable\": true\n    }\n  },\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-airport-urls-contract-schema.json
tags:
- Aviation
- Flights
- Aerospace
- Flight Data
- Airport Data
title: AirportUrlsContract
---
