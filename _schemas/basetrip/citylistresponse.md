---
description: ''
layout: schema
name: CityListResponse
properties_list:
- description: ''
  name: cities
  type: array
- description: ''
  name: count
  type: integer
provider_name: Basetrip
provider_slug: basetrip
schema_file: json-schema/citylistresponse.json
slug: citylistresponse
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/basetrip/refs/heads/main/json-schema/citylistresponse.json\",\n  \"title\": \"CityListResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cities\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/City\"\n      }\n    },\n    \"count\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/basetrip/refs/heads/main/json-schema/citylistresponse.json
tags:
- Cities
- Countries
- Health
- Safety
- Travel
- Visa
title: CityListResponse
---
