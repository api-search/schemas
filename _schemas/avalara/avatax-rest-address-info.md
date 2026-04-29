---
description: AddressInfo schema from Avalara API
layout: schema
name: AddressInfo
properties_list:
- description: Street address line 1
  name: line1
  type: string
- description: Street address line 2
  name: line2
  type: string
- description: Street address line 3
  name: line3
  type: string
- description: City name
  name: city
  type: string
- description: State, province, or region code
  name: region
  type: string
- description: Postal code or ZIP code
  name: postalCode
  type: string
- description: Two-character ISO 3166 country code
  name: country
  type: string
- description: ''
  name: latitude
  type: number
- description: ''
  name: longitude
  type: number
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/avatax-rest-address-info-schema.json
slug: avatax-rest-address-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avatax-rest-address-info-schema.json\",\n  \"title\": \"AddressInfo\",\n  \"description\": \"AddressInfo schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"line1\": {\n      \"type\": \"string\",\n      \"description\": \"Street address line 1\"\n    },\n    \"line2\": {\n      \"type\": \"string\",\n      \"description\": \"Street address line 2\"\n    },\n    \"line3\": {\n      \"type\": \"string\",\n      \"description\": \"Street address line 3\"\n    },\n    \"city\": {\n      \"type\": \"string\",\n      \"description\": \"City name\"\n    },\n    \"region\": {\n      \"type\": \"string\",\n      \"description\": \"State, province, or region code\"\n    },\n    \"postalCode\": {\n      \"type\": \"string\",\n      \"description\": \"Postal code or ZIP code\"\n    },\n    \"\
  country\": {\n      \"type\": \"string\",\n      \"description\": \"Two-character ISO 3166 country code\"\n    },\n    \"latitude\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n    \"longitude\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avatax-rest-address-info-schema.json
tags:
- Taxes
title: AddressInfo
---
