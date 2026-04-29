---
description: A coach station in the BlaBlaCar Bus network
layout: schema
name: Station
properties_list:
- description: Unique station identifier
  name: id
  type: string
- description: Station name
  name: name
  type: string
- description: City where the station is located
  name: city
  type: string
- description: ISO 3166-1 alpha-2 country code
  name: country_code
  type: string
- description: Geographic latitude
  name: latitude
  type: number
- description: Geographic longitude
  name: longitude
  type: number
- description: Full street address
  name: address
  type: string
provider_name: BlaBlaCar Bus API
provider_slug: blablacar-bus-api
schema_file: json-schema/blablacar-bus-api-station-schema.json
slug: blablacar-bus-api-station
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/blablacar-bus-api/refs/heads/main/json-schema/blablacar-bus-api-station-schema.json\",\n  \"title\": \"Station\",\n  \"description\": \"A coach station in the BlaBlaCar Bus network\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique station identifier\",\n      \"example\": \"FRTLS\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Station name\",\n      \"example\": \"Paris Bercy\"\n    },\n    \"city\": {\n      \"type\": \"string\",\n      \"description\": \"City where the station is located\",\n      \"example\": \"Paris\"\n    },\n    \"country_code\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 3166-1 alpha-2 country code\",\n      \"example\": \"FR\"\n    },\n    \"latitude\": {\n      \"type\": \"number\",\n      \"description\"\
  : \"Geographic latitude\",\n      \"example\": 48.8397\n    },\n    \"longitude\": {\n      \"type\": \"number\",\n      \"description\": \"Geographic longitude\",\n      \"example\": 2.3826\n    },\n    \"address\": {\n      \"type\": \"string\",\n      \"description\": \"Full street address\",\n      \"example\": \"210 Quai de Bercy, 75012 Paris\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"name\",\n    \"city\",\n    \"country_code\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/blablacar-bus-api/refs/heads/main/json-schema/blablacar-bus-api-station-schema.json
tags:
- Booking
- Buses
- Coach
- Europe
- Mobility
- Ticketing
- Transportation
- Travel
title: Station
---
