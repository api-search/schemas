---
description: detail information of the virtual card
layout: schema
name: VirtualCreditCardDetails
properties_list: []
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/flight-order-management-virtual-credit-card-details-schema.json
slug: flight-order-management-virtual-credit-card-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-order-management-virtual-credit-card-details-schema.json\",\n  \"title\": \"VirtualCreditCardDetails\",\n  \"description\": \"detail information of the virtual card\",\n  \"allOf\": [\n    {\n      \"$ref\": \"#/definitions/CreditCardCommon\"\n    },\n    {\n      \"$ref\": \"#/definitions/ElementaryPrice\"\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-order-management-virtual-credit-card-details-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: VirtualCreditCardDetails
---
