---
description: File schema from Adyen API
layout: schema
name: File
properties_list:
- description: The certificate content converted to a Base64-encoded string.
  name: data
  type: string
- description: The name of the certificate. Must be unique across Wi-Fi profiles.
  name: name
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-file-schema.json
slug: management-file
source_filename: management-file-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-file-schema.json\",\n  \"title\": \"File\",\n  \"description\": \"File schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"description\": \"The certificate content converted to a Base64-encoded string.\",\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"description\": \"The name of the certificate. Must be unique across Wi-Fi profiles.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"data\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-file-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: File
---
