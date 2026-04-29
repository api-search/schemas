---
description: A physical address.
layout: schema
name: Address
properties_list:
- description: Street address line.
  name: streetAddress
  type: string
- description: Additional street address information.
  name: streetAddress2
  type: string
- description: City name.
  name: city
  type: string
- description: State, province, or region.
  name: state
  type: string
- description: Postal or ZIP code.
  name: postalCode
  type: string
- description: ISO 3166-1 alpha-2 country code.
  name: country
  type: string
provider_name: Indeed
provider_slug: indeed
schema_file: json-schema/indeed-employer-address-schema.json
slug: indeed-employer-address
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Address\",\n  \"type\": \"object\",\n  \"description\": \"A physical address.\",\n  \"properties\": {\n    \"streetAddress\": {\n      \"type\": \"string\",\n      \"description\": \"Street address line.\"\n    },\n    \"streetAddress2\": {\n      \"type\": \"string\",\n      \"description\": \"Additional street address information.\"\n    },\n    \"city\": {\n      \"type\": \"string\",\n      \"description\": \"City name.\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"State, province, or region.\"\n    },\n    \"postalCode\": {\n      \"type\": \"string\",\n      \"description\": \"Postal or ZIP code.\"\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 3166-1 alpha-2 country code.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/indeed/refs/heads/main/json-schema/indeed-employer-address-schema.json
tags:
- Careers
- Employment
- Hiring
- Job Search
- Jobs
- Recruiting
title: Address
---
