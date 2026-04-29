---
description: ''
layout: schema
name: Country
properties_list:
- description: Country name in English
  name: name
  type: string
- description: URL-friendly country slug
  name: slug
  type: string
- description: ISO alpha-2 country code
  name: code
  type: string
- description: Continent name
  name: continent
  type: string
provider_name: Basetrip
provider_slug: basetrip
schema_file: json-schema/country.json
slug: country
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/basetrip/refs/heads/main/json-schema/country.json\",\n  \"title\": \"Country\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Country name in English\"\n    },\n    \"slug\": {\n      \"type\": \"string\",\n      \"description\": \"URL-friendly country slug\"\n    },\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"ISO alpha-2 country code\"\n    },\n    \"continent\": {\n      \"type\": \"string\",\n      \"description\": \"Continent name\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"slug\",\n    \"code\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/basetrip/refs/heads/main/json-schema/country.json
tags:
- Cities
- Countries
- Health
- Safety
- Travel
- Visa
title: Country
---
