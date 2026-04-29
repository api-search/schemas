---
description: Error response containing one or more error details.
layout: schema
name: ErrorResponse
properties_list:
- description: Array of error details.
  name: errors
  type: array
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/airline-code-lookup-errorresponse-schema.json
slug: airline-code-lookup-errorresponse
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"ErrorResponse\",\n  \"description\": \"Error response containing one or more error details.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"errors\": {\n      \"type\": \"array\",\n      \"description\": \"Array of error details.\",\n      \"items\": {\n        \"$ref\": \"#/definitions/Issue\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/airline-code-lookup-errorresponse-schema.json
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
title: ErrorResponse
---
