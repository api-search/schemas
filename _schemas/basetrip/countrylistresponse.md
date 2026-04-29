---
description: ''
layout: schema
name: CountryListResponse
properties_list:
- description: ''
  name: countries
  type: array
- description: Total number of countries
  name: count
  type: integer
provider_name: Basetrip
provider_slug: basetrip
schema_file: json-schema/countrylistresponse.json
slug: countrylistresponse
source_filename: countrylistresponse.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/basetrip/refs/heads/main/json-schema/countrylistresponse.json\",\n  \"title\": \"CountryListResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"countries\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Country\"\n      }\n    },\n    \"count\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of countries\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/basetrip/refs/heads/main/json-schema/countrylistresponse.json
tags:
- Cities
- Countries
- Health
- Safety
- Travel
- Visa
title: CountryListResponse
---
