---
description: Includes the common name of the carrier (Operating or Marketing)
layout: schema
name: carrier
properties_list:
- description: Common name of the organization.
  name: name
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/trip-parser-carrier-schema.json
slug: trip-parser-carrier
source_filename: trip-parser-carrier-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"carrier\",\n  \"description\": \"Includes the common name of the carrier (Operating or Marketing)\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Common name of the organization.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/trip-parser-carrier-schema.json
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
title: carrier
---
