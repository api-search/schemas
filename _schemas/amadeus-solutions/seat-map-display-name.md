---
description: name
layout: schema
name: Name
properties_list: []
provider_name: Amadeus Solutions
provider_slug: amadeus-solutions
schema_file: json-schema/seat-map-display-name-schema.json
slug: seat-map-display-name
source_filename: seat-map-display-name-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/seat-map-display-name-schema.json\",\n  \"title\": \"Name\",\n  \"description\": \"name\",\n  \"allOf\": [\n    {\n      \"$ref\": \"#/definitions/BaseName\"\n    },\n    {\n      \"type\": \"object\",\n      \"properties\": {\n        \"secondLastName\": {\n          \"description\": \"second last name\",\n          \"type\": \"string\"\n        }\n      }\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/seat-map-display-name-schema.json
tags:
- Airlines
- Booking
- Flights
- GDS
- Hotels
- Travel
- Travel Technology
title: Name
---
