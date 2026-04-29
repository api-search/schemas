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
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/flight-order-management-automated-process-common-schema.json
slug: flight-order-management-automated-process-common
source_filename: flight-order-management-automated-process-common-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-order-management-automated-process-common-schema.json\",\n  \"title\": \"AutomatedProcessCommon\",\n  \"description\": \"Provides information on ticketing arrangements and Amadeus Time Limits\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"code\": {\n      \"$ref\": \"#/definitions/AutomatedProcessCode\"\n    },\n    \"queue\": {\n      \"title\": \"Queue\",\n      \"type\": \"object\",\n      \"description\": \"Identifies the queue onto which PNR must be automatically placed upon process execution.\",\n      \"properties\": {\n        \"number\": {\n          \"type\": \"string\"\n        },\n        \"category\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"text\": {\n      \"type\": \"string\",\n      \"description\": \"Free text\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-order-management-automated-process-common-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: AutomatedProcessCommon
---
