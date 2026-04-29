---
description: automatic process applied to the Order
layout: schema
name: AutomatedProcess
properties_list: []
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/flight-order-management-automated-process-schema.json
slug: flight-order-management-automated-process
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-order-management-automated-process-schema.json\",\n  \"title\": \"AutomatedProcess\",\n  \"description\": \"automatic process applied to the Order\",\n  \"allOf\": [\n    {\n      \"$ref\": \"#/definitions/AutomatedProcessCommon\"\n    },\n    {\n      \"type\": \"object\",\n      \"properties\": {\n        \"delay\": {\n          \"description\": \"Delay before applying process in days\",\n          \"type\": \"string\"\n        },\n        \"officeId\": {\n          \"description\": \"Office into which the process must be triggered.\",\n          \"type\": \"string\",\n          \"example\": \"NCE1A0955\"\n        },\n        \"dateTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Datetime limit at which the process takes action\
  \ in case issuance is not done.\"\n        }\n      }\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-order-management-automated-process-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: AutomatedProcess
---
