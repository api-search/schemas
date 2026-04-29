---
description: PinChangeResponse schema from Adyen API
layout: schema
name: PinChangeResponse
properties_list:
- description: The pin change status.
  name: status
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-pin-change-response-schema.json
slug: configuration-pin-change-response
source_filename: configuration-pin-change-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-pin-change-response-schema.json\",\n  \"title\": \"PinChangeResponse\",\n  \"description\": \"PinChangeResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"description\": \"The pin change status.\",\n      \"enum\": [\n        \"completed\",\n        \"pending\",\n        \"unavailable\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-pin-change-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PinChangeResponse
---
