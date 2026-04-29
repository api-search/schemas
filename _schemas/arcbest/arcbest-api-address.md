---
description: ''
layout: schema
name: Address
properties_list:
- description: Company or person name
  name: name
  type: string
- description: Street address
  name: address
  type: string
- description: City
  name: city
  type: string
- description: State abbreviation
  name: state
  type: string
- description: ZIP code
  name: zip
  type: string
- description: Country code (ISO 3166-1 alpha-2)
  name: country
  type: string
provider_name: ArcBest
provider_slug: arcbest
schema_file: json-schema/arcbest-api-address-schema.json
slug: arcbest-api-address
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Company or person name\",\n      \"example\": \"ACME Corp\"\n    },\n    \"address\": {\n      \"type\": \"string\",\n      \"description\": \"Street address\",\n      \"example\": \"123 Main St\"\n    },\n    \"city\": {\n      \"type\": \"string\",\n      \"description\": \"City\",\n      \"example\": \"Benton\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"State abbreviation\",\n      \"example\": \"AR\"\n    },\n    \"zip\": {\n      \"type\": \"string\",\n      \"description\": \"ZIP code\",\n      \"example\": \"72015\"\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"description\": \"Country code (ISO 3166-1 alpha-2)\",\n      \"example\": \"US\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/arcbest/refs/heads/main/json-schema/arcbest-api-address-schema.json\"\
  ,\n  \"title\": \"Address\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/arcbest/refs/heads/main/json-schema/arcbest-api-address-schema.json
tags:
- Logistics
- Freight
- LTL
- Supply Chain
- Shipping
- Transportation
title: Address
---
