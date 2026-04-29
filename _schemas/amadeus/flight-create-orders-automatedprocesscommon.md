---
description: Provides information on ticketing arrangements and Amadeus Time Limits
layout: schema
name: AutomatedProcessCommon
properties_list:
- description: ''
  name: code
  type: object
- description: Identifies the queue onto which PNR must be automatically placed upon process execution.
  name: queue
  type: object
- description: Free text
  name: text
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-create-orders-automatedprocesscommon-schema.json
slug: flight-create-orders-automatedprocesscommon
source_filename: flight-create-orders-automatedprocesscommon-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"AutomatedProcessCommon\",\n  \"description\": \"Provides information on ticketing arrangements and Amadeus Time Limits\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"code\": {\n      \"$ref\": \"#/definitions/AutomatedProcessCode\"\n    },\n    \"queue\": {\n      \"type\": \"object\",\n      \"description\": \"Identifies the queue onto which PNR must be automatically placed upon process execution.\",\n      \"properties\": {\n        \"number\": {\n          \"type\": \"string\"\n        },\n        \"category\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"text\": {\n      \"type\": \"string\",\n      \"description\": \"Free text\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/flight-create-orders-automatedprocesscommon-schema.json
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
title: AutomatedProcessCommon
---
