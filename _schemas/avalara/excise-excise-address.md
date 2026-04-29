---
description: ExciseAddress schema from Avalara API
layout: schema
name: ExciseAddress
properties_list:
- description: ''
  name: line1
  type: string
- description: ''
  name: line2
  type: string
- description: ''
  name: city
  type: string
- description: State or province code
  name: region
  type: string
- description: ''
  name: postalCode
  type: string
- description: ISO 3166 country code
  name: country
  type: string
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/excise-excise-address-schema.json
slug: excise-excise-address
source_filename: excise-excise-address-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/excise-excise-address-schema.json\",\n  \"title\": \"ExciseAddress\",\n  \"description\": \"ExciseAddress schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"line1\": {\n      \"type\": \"string\"\n    },\n    \"line2\": {\n      \"type\": \"string\"\n    },\n    \"city\": {\n      \"type\": \"string\"\n    },\n    \"region\": {\n      \"type\": \"string\",\n      \"description\": \"State or province code\"\n    },\n    \"postalCode\": {\n      \"type\": \"string\"\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 3166 country code\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/excise-excise-address-schema.json
tags:
- Taxes
title: ExciseAddress
---
