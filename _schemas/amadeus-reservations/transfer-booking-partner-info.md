---
description: Information about partner/subprovider. Below settings configuration is not applicable for sub-provider. Fields 'code', 'name' and 'logoUrl' are not mandatory for sub-provider.
layout: schema
name: PartnerInfo
properties_list:
- description: ''
  name: serviceProvider
  type: object
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/transfer-booking-partner-info-schema.json
slug: transfer-booking-partner-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/transfer-booking-partner-info-schema.json\",\n  \"title\": \"PartnerInfo\",\n  \"description\": \"Information about partner/subprovider. Below settings configuration is not applicable for sub-provider. Fields 'code', 'name' and 'logoUrl' are not mandatory for sub-provider.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"serviceProvider\": {\n      \"$ref\": \"#/definitions/ServiceProvider\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/transfer-booking-partner-info-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: PartnerInfo
---
