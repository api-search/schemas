---
description: ShippingLocationsResponse schema from Adyen API
layout: schema
name: ShippingLocationsResponse
properties_list:
- description: Physical locations where orders can be shipped to.
  name: data
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-shipping-locations-response-schema.json
slug: management-shipping-locations-response
source_filename: management-shipping-locations-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-shipping-locations-response-schema.json\",\n  \"title\": \"ShippingLocationsResponse\",\n  \"description\": \"ShippingLocationsResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"description\": \"Physical locations where orders can be shipped to.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ShippingLocation\"\n      },\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-shipping-locations-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ShippingLocationsResponse
---
