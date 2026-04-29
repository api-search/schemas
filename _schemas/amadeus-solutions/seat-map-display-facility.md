---
description: Facility schema
layout: schema
name: Facility
properties_list:
- description: Facility code, as described in the facility dictionary
  name: code
  type: string
- description: ''
  name: column
  type: string
- description: ''
  name: row
  type: string
- description: Position is either front, rear or seat (in case the facility takes the place of a seat)
  name: position
  type: string
- description: ''
  name: coordinates
  type: object
provider_name: Amadeus Solutions
provider_slug: amadeus-solutions
schema_file: json-schema/seat-map-display-facility-schema.json
slug: seat-map-display-facility
source_filename: seat-map-display-facility-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/seat-map-display-facility-schema.json\",\n  \"title\": \"Facility\",\n  \"description\": \"Facility schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"code\": {\n      \"description\": \"Facility code, as described in the facility dictionary\",\n      \"type\": \"string\"\n    },\n    \"column\": {\n      \"type\": \"string\"\n    },\n    \"row\": {\n      \"type\": \"string\"\n    },\n    \"position\": {\n      \"type\": \"string\",\n      \"description\": \"Position is either front, rear or seat (in case the facility takes the place of a seat)\",\n      \"enum\": [\n        \"FRONT\",\n        \"REAR\",\n        \"SEAT\"\n      ]\n    },\n    \"coordinates\": {\n      \"$ref\": \"#/definitions/Coordinates\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/seat-map-display-facility-schema.json
tags:
- Airlines
- Booking
- Flights
- GDS
- Hotels
- Travel
- Travel Technology
title: Facility
---
