---
description: ticket information
layout: schema
name: AirTravelDocument
properties_list: []
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/flight-create-orders-air-travel-document-schema.json
slug: flight-create-orders-air-travel-document
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-create-orders-air-travel-document-schema.json\",\n  \"title\": \"AirTravelDocument\",\n  \"description\": \"ticket information\",\n  \"allOf\": [\n    {\n      \"$ref\": \"#/definitions/AirTravelDocumentCommon\"\n    },\n    {\n      \"type\": \"object\",\n      \"properties\": {\n        \"travelerId\": {\n          \"type\": \"string\",\n          \"description\": \"id of the impacted traveler\",\n          \"example\": \"1\"\n        },\n        \"segmentIds\": {\n          \"description\": \"Ids of the impacted segments\",\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"example\": \"1\"\n        }\n      }\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-create-orders-air-travel-document-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: AirTravelDocument
---
