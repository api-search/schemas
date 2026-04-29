---
description: Shipping address for an order
layout: schema
name: ShippingAddress
properties_list:
- description: Street address
  name: street
  type: string
- description: City name
  name: city
  type: string
- description: State or province code
  name: state
  type: string
- description: Postal/ZIP code
  name: zip
  type: string
- description: Country code (ISO 3166-1 alpha-2)
  name: country
  type: string
provider_name: 3M
provider_slug: 3m
schema_file: json-schema/3m-partner-supplier-api-shipping-address-schema.json
slug: 3m-partner-supplier-api-shipping-address
source_filename: 3m-partner-supplier-api-shipping-address-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/3m/refs/heads/main/json-schema/3m-partner-supplier-api-shipping-address-schema.json\",\n  \"title\": \"ShippingAddress\",\n  \"description\": \"Shipping address for an order\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"street\": {\n      \"type\": \"string\",\n      \"description\": \"Street address\",\n      \"example\": \"3M Center\"\n    },\n    \"city\": {\n      \"type\": \"string\",\n      \"description\": \"City name\",\n      \"example\": \"St. Paul\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"State or province code\",\n      \"example\": \"MN\"\n    },\n    \"zip\": {\n      \"type\": \"string\",\n      \"description\": \"Postal/ZIP code\",\n      \"example\": \"55144\"\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"description\": \"Country code (ISO 3166-1 alpha-2)\",\n\
  \      \"example\": \"US\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/3m/refs/heads/main/json-schema/3m-partner-supplier-api-shipping-address-schema.json
tags:
- Industrial
- Manufacturing
- Supply Chain
title: ShippingAddress
---
