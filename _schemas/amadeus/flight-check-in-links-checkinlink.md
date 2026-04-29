---
description: ''
layout: schema
name: CheckinLink
properties_list:
- description: the resource name
  name: type
  type: string
- description: identifier of the resource
  name: id
  type: string
- description: direct URL to the relevant page
  name: href
  type: string
- description: indicates the type of channel supported by the URL
  name: channel
  type: string
- description: list of URL parameters with descriptive information such as description and/or type and/or format
  name: parameters
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-check-in-links-checkinlink-schema.json
slug: flight-check-in-links-checkinlink
source_filename: flight-check-in-links-checkinlink-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"CheckinLink\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"the resource name\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"identifier of the resource\"\n    },\n    \"href\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"direct URL to the relevant page\"\n    },\n    \"channel\": {\n      \"type\": \"string\",\n      \"description\": \"indicates the type of channel supported by the URL\",\n      \"enum\": [\n        \"Mobile\",\n        \"Web\",\n        \"All\"\n      ]\n    },\n    \"parameters\": {\n      \"description\": \"list of URL parameters with descriptive information such as description and/or type and/or format\"\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"id\",\n    \"href\",\n    \"channel\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/flight-check-in-links-checkinlink-schema.json
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
title: CheckinLink
---
