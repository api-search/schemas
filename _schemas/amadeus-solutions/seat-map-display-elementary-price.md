---
description: elementaryPrice
layout: schema
name: ElementaryPrice
properties_list:
- description: Amount of the fare. could be alpha numeric. Ex- 500.20 or 514.13A, 'A'signifies additional collection.
  name: amount
  type: string
- description: Currency type of the fare.
  name: currencyCode
  type: string
provider_name: Amadeus Solutions
provider_slug: amadeus-solutions
schema_file: json-schema/seat-map-display-elementary-price-schema.json
slug: seat-map-display-elementary-price
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/seat-map-display-elementary-price-schema.json\",\n  \"title\": \"ElementaryPrice\",\n  \"description\": \"elementaryPrice\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"amount\": {\n      \"type\": \"string\",\n      \"description\": \"Amount of the fare. could be alpha numeric. Ex- 500.20 or 514.13A, 'A'signifies additional collection.\"\n    },\n    \"currencyCode\": {\n      \"type\": \"string\",\n      \"description\": \"Currency type of the fare.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/seat-map-display-elementary-price-schema.json
tags:
- Airlines
- Booking
- Flights
- GDS
- Hotels
- Travel
- Travel Technology
title: ElementaryPrice
---
