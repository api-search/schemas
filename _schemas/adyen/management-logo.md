---
description: Logo schema from Adyen API
layout: schema
name: Logo
properties_list:
- description: The image file, converted to a Base64-encoded string, of the logo to be shown on the terminal.
  name: data
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-logo-schema.json
slug: management-logo
source_filename: management-logo-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-logo-schema.json\",\n  \"title\": \"Logo\",\n  \"description\": \"Logo schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"description\": \"The image file, converted to a Base64-encoded string, of the logo to be shown on the terminal.\",\n      \"maxLength\": 350000,\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-logo-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: Logo
---
