---
description: Physical or mailing address
layout: schema
name: Address
properties_list:
- description: Type of address
  name: addressType
  type: string
- description: First line of address
  name: addressLine1
  type: string
- description: Second line of address
  name: addressLine2
  type: string
- description: City name
  name: city
  type: string
- description: State or province
  name: state
  type: string
- description: Postal or ZIP code
  name: postCode
  type: string
- description: Country code (ISO 3166)
  name: country
  type: string
provider_name: Temenos Transact
provider_slug: temenos-transact
schema_file: json-schema/temenos-transact-core-banking-address-schema.json
slug: temenos-transact-core-banking-address
source_filename: temenos-transact-core-banking-address-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Address\",\n  \"type\": \"object\",\n  \"description\": \"Physical or mailing address\",\n  \"properties\": {\n    \"addressType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of address\"\n    },\n    \"addressLine1\": {\n      \"type\": \"string\",\n      \"description\": \"First line of address\"\n    },\n    \"addressLine2\": {\n      \"type\": \"string\",\n      \"description\": \"Second line of address\"\n    },\n    \"city\": {\n      \"type\": \"string\",\n      \"description\": \"City name\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"State or province\"\n    },\n    \"postCode\": {\n      \"type\": \"string\",\n      \"description\": \"Postal or ZIP code\"\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"description\": \"Country code (ISO 3166)\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/temenos-transact/refs/heads/main/json-schema/temenos-transact-core-banking-address-schema.json
tags:
- Banking
- Core Banking
- Digital Banking
- Enterprise
- Financial Services
- Fintech
title: Address
---
