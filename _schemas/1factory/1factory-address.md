---
description: Address schema from 1Factory API
layout: schema
name: Address
properties_list:
- description: Street address.
  name: street
  type: string
- description: City name.
  name: city
  type: string
- description: State or province.
  name: state
  type: string
- description: Postal or ZIP code.
  name: postal_code
  type: string
- description: Country code (ISO 3166-1 alpha-2 format recommended).
  name: country
  type: string
provider_name: 1Factory
provider_slug: 1factory
schema_file: json-schema/1factory-address-schema.json
slug: 1factory-address
source_filename: 1factory-address-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/1factory/refs/heads/main/json-schema/1factory-address-schema.json\",\n  \"title\": \"Address\",\n  \"description\": \"Address schema from 1Factory API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"street\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"maxLength\": 255,\n      \"description\": \"Street address.\",\n      \"example\": \"Washington\"\n    },\n    \"city\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"maxLength\": 100,\n      \"description\": \"City name.\",\n      \"example\": \"Jefferson\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"maxLength\": 50,\n      \"description\": \"State or province.\",\n      \"example\": \"Il\"\n    },\n    \"postal_code\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"maxLength\":\
  \ 20,\n      \"description\": \"Postal or ZIP code.\",\n      \"example\": \"60134\"\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"maxLength\": 10,\n      \"description\": \"Country code (ISO 3166-1 alpha-2 format recommended).\",\n      \"example\": \"US\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/1factory/refs/heads/main/json-schema/1factory-address-schema.json
tags:
- Analytics
- Data Collection
- Manufacturing
- Monitoring
- Quality
title: Address
---
