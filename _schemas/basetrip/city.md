---
description: ''
layout: schema
name: City
properties_list:
- description: City name
  name: name
  type: string
- description: URL-friendly city slug
  name: slug
  type: string
- description: Country alpha-2 code
  name: country
  type: string
provider_name: Basetrip
provider_slug: basetrip
schema_file: json-schema/city.json
slug: city
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/basetrip/refs/heads/main/json-schema/city.json\",\n  \"title\": \"City\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"City name\"\n    },\n    \"slug\": {\n      \"type\": \"string\",\n      \"description\": \"URL-friendly city slug\"\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"description\": \"Country alpha-2 code\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"slug\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/basetrip/refs/heads/main/json-schema/city.json
tags:
- Cities
- Countries
- Health
- Safety
- Travel
- Visa
title: City
---
