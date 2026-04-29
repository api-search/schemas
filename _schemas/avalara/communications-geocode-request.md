---
description: GeocodeRequest schema from Avalara API
layout: schema
name: GeocodeRequest
properties_list:
- description: Reference ID
  name: ref
  type: string
- description: Whether to return CASS-certified address
  name: cass
  type: boolean
- description: Street address
  name: addr
  type: string
- description: ''
  name: city
  type: string
- description: State abbreviation
  name: st
  type: string
- description: ZIP code
  name: zip
  type: string
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/communications-geocode-request-schema.json
slug: communications-geocode-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/communications-geocode-request-schema.json\",\n  \"title\": \"GeocodeRequest\",\n  \"description\": \"GeocodeRequest schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ref\": {\n      \"type\": \"string\",\n      \"description\": \"Reference ID\"\n    },\n    \"cass\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to return CASS-certified address\"\n    },\n    \"addr\": {\n      \"type\": \"string\",\n      \"description\": \"Street address\"\n    },\n    \"city\": {\n      \"type\": \"string\"\n    },\n    \"st\": {\n      \"type\": \"string\",\n      \"description\": \"State abbreviation\"\n    },\n    \"zip\": {\n      \"type\": \"string\",\n      \"description\": \"ZIP code\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/communications-geocode-request-schema.json
tags:
- Taxes
title: GeocodeRequest
---
