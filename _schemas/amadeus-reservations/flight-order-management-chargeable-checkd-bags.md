---
description: Details of chargeable checked bags
layout: schema
name: ChargeableCheckdBags
properties_list: []
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/flight-order-management-chargeable-checkd-bags-schema.json
slug: flight-order-management-chargeable-checkd-bags
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-order-management-chargeable-checkd-bags-schema.json\",\n  \"title\": \"ChargeableCheckdBags\",\n  \"description\": \"Details of chargeable checked bags\",\n  \"allOf\": [\n    {\n      \"$ref\": \"#/definitions/BaggageAllowance\"\n    },\n    {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"description\": \"Id of the chargeable bag\",\n          \"type\": \"string\",\n          \"example\": \"1\"\n        }\n      }\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-order-management-chargeable-checkd-bags-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: ChargeableCheckdBags
---
