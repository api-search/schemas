---
description: Information about partner/subprovider. Below settings configuration is not applicable for sub-provider. Fields 'code', 'name' and 'logoUrl' are not mandatory for sub-provider.
layout: schema
name: PartnerInfo
properties_list:
- description: ''
  name: serviceProvider
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/transfer-booking-partnerinfo-schema.json
slug: transfer-booking-partnerinfo
source_filename: transfer-booking-partnerinfo-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"PartnerInfo\",\n  \"description\": \"Information about partner/subprovider. Below settings configuration is not applicable for sub-provider. Fields 'code', 'name' and 'logoUrl' are not mandatory for sub-provider.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"serviceProvider\": {\n      \"$ref\": \"#/definitions/ServiceProvider\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/transfer-booking-partnerinfo-schema.json
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
title: PartnerInfo
---
