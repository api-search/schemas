---
description: A postal address.
layout: schema
name: AddressObject
properties_list:
- description: Primary street address line.
  name: line1
  type: string
- description: Secondary address line (apartment, suite, unit, etc.).
  name: line2
  type: string
- description: City or locality.
  name: city
  type: string
- description: State, province, or region code.
  name: state
  type: string
- description: Postal or ZIP code.
  name: zipcode
  type: string
- description: ISO 3166-1 alpha-2 country code.
  name: country
  type: string
provider_name: affirm
provider_slug: affirm
schema_file: json-schema/checkout-address-object-schema.json
slug: checkout-address-object
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/affirm/refs/heads/main/json-schema/checkout-address-object-schema.json\",\n  \"title\": \"AddressObject\",\n  \"description\": \"A postal address.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"line1\": {\n      \"type\": \"string\",\n      \"description\": \"Primary street address line.\",\n      \"example\": \"example_value\"\n    },\n    \"line2\": {\n      \"type\": \"string\",\n      \"description\": \"Secondary address line (apartment, suite, unit, etc.).\",\n      \"example\": \"example_value\"\n    },\n    \"city\": {\n      \"type\": \"string\",\n      \"description\": \"City or locality.\",\n      \"example\": \"example_value\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"State, province, or region code.\",\n      \"example\": \"example_value\"\n    },\n    \"zipcode\": {\n      \"type\": \"\
  string\",\n      \"description\": \"Postal or ZIP code.\",\n      \"example\": \"example_value\"\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 3166-1 alpha-2 country code.\",\n      \"example\": \"example_value\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/affirm/refs/heads/main/json-schema/checkout-address-object-schema.json
tags: []
title: AddressObject
---
