---
description: Australian postal address
layout: schema
name: Address
properties_list:
- description: Street address including number
  name: street
  type: string
- description: Suburb name
  name: suburb
  type: string
- description: Australian state or territory code
  name: state
  type: string
- description: Australian postcode
  name: postcode
  type: string
provider_name: Allianz
provider_slug: allianz-docs
schema_file: json-schema/api-connect-address-schema.json
slug: api-connect-address
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/allianz-docs/refs/heads/main/json-schema/api-connect-address-schema.json\",\n  \"title\": \"Address\",\n  \"description\": \"Australian postal address\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"street\": {\n      \"type\": \"string\",\n      \"description\": \"Street address including number\",\n      \"example\": \"123 Main St\"\n    },\n    \"suburb\": {\n      \"type\": \"string\",\n      \"description\": \"Suburb name\",\n      \"example\": \"Sydney\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"Australian state or territory code\",\n      \"enum\": [\n        \"NSW\",\n        \"VIC\",\n        \"QLD\",\n        \"WA\",\n        \"SA\",\n        \"TAS\",\n        \"ACT\",\n        \"NT\"\n      ],\n      \"example\": \"NSW\"\n    },\n    \"postcode\": {\n      \"type\": \"string\",\n      \"\
  description\": \"Australian postcode\",\n      \"example\": \"2000\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/allianz-docs/refs/heads/main/json-schema/api-connect-address-schema.json
tags:
- Financial Services
- Insurance
- Asset Management
title: Address
---
