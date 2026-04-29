---
description: Airport schedule contract
layout: schema
name: AirportFidsContract
properties_list:
- description: Departing flights
  name: departures
  type: array
- description: Arriving flights
  name: arrivals
  type: array
provider_name: AeroDataBox
provider_slug: aerodatabox
schema_file: json-schema/aerodatabox-airport-fids-contract-schema.json
slug: aerodatabox-airport-fids-contract
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-airport-fids-contract-schema.json\",\n  \"title\": \"AirportFidsContract\",\n  \"description\": \"Airport schedule contract\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"departures\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/AirportFlightContract\"\n      },\n      \"description\": \"Departing flights\",\n      \"nullable\": true\n    },\n    \"arrivals\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/AirportFlightContract\"\n      },\n      \"description\": \"Arriving flights\",\n      \"nullable\": true\n    }\n  },\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-airport-fids-contract-schema.json
tags:
- Aviation
- Flights
- Aerospace
- Flight Data
- Airport Data
title: AirportFidsContract
---
