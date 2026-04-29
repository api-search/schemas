---
description: the purpose for which this contact is to be used. - STANDARD for standard use, comunication, advertissement etc... - INVOICE for your invoice contact, usually its your billing adress. it's mandatory in france when you buy online - STANDARD_WITHOUT_TRANSMISSION is standard contact that are not share with third party outside of Amadeus
layout: schema
name: ContactPurpose
properties_list: []
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/flight-create-orders-contact-purpose-schema.json
slug: flight-create-orders-contact-purpose
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-create-orders-contact-purpose-schema.json\",\n  \"title\": \"ContactPurpose\",\n  \"description\": \"the purpose for which this contact is to be used.\\n - STANDARD for standard use, comunication, advertissement etc...\\n - INVOICE for your invoice contact, usually its your billing adress. it's mandatory in france when you buy online\\n - STANDARD_WITHOUT_TRANSMISSION is standard contact that are not share with third party outside of Amadeus\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"STANDARD\",\n    \"INVOICE\",\n    \"STANDARD_WITHOUT_TRANSMISSION\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-create-orders-contact-purpose-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: ContactPurpose
---
