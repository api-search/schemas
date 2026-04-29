---
description: FlightDataGeneralAvailabilityContract schema from AeroDataBox API
layout: schema
name: FlightDataGeneralAvailabilityContract
properties_list:
- description: Date of the oldest flight stored (based on scheduled local times) If not specified, no flight data available
  name: minAvailableLocalDate
  type: string
- description: Date of the most recent flight stored (based on scheduled local times) If not specified, no flight data available
  name: maxAvailableLocalDate
  type: string
provider_name: AeroDataBox
provider_slug: aerodatabox
schema_file: json-schema/aerodatabox-flight-data-general-availability-contract-schema.json
slug: aerodatabox-flight-data-general-availability-contract
source_filename: aerodatabox-flight-data-general-availability-contract-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-flight-data-general-availability-contract-schema.json\",\n  \"title\": \"FlightDataGeneralAvailabilityContract\",\n  \"description\": \"FlightDataGeneralAvailabilityContract schema from AeroDataBox API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"minAvailableLocalDate\": {\n      \"type\": \"string\",\n      \"description\": \"Date of the oldest flight stored (based on scheduled local times)\\r\\nIf not specified, no flight data available\",\n      \"format\": \"date-time\",\n      \"nullable\": true\n    },\n    \"maxAvailableLocalDate\": {\n      \"type\": \"string\",\n      \"description\": \"Date of the most recent flight stored (based on scheduled local times)\\r\\nIf not specified, no flight data available\",\n      \"format\": \"date-time\",\n      \"nullable\": true\n    }\n\
  \  },\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-flight-data-general-availability-contract-schema.json
tags:
- Aviation
- Flights
- Aerospace
- Flight Data
- Airport Data
title: FlightDataGeneralAvailabilityContract
---
