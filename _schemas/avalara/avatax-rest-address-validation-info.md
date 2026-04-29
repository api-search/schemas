---
description: AddressValidationInfo schema from Avalara API
layout: schema
name: AddressValidationInfo
properties_list:
- description: ''
  name: line1
  type: string
- description: ''
  name: line2
  type: string
- description: ''
  name: line3
  type: string
- description: ''
  name: city
  type: string
- description: ''
  name: region
  type: string
- description: ''
  name: postalCode
  type: string
- description: ''
  name: country
  type: string
- description: ''
  name: textCase
  type: string
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/avatax-rest-address-validation-info-schema.json
slug: avatax-rest-address-validation-info
source_filename: avatax-rest-address-validation-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avatax-rest-address-validation-info-schema.json\",\n  \"title\": \"AddressValidationInfo\",\n  \"description\": \"AddressValidationInfo schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"line1\": {\n      \"type\": \"string\"\n    },\n    \"line2\": {\n      \"type\": \"string\"\n    },\n    \"line3\": {\n      \"type\": \"string\"\n    },\n    \"city\": {\n      \"type\": \"string\"\n    },\n    \"region\": {\n      \"type\": \"string\"\n    },\n    \"postalCode\": {\n      \"type\": \"string\"\n    },\n    \"country\": {\n      \"type\": \"string\"\n    },\n    \"textCase\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Default\",\n        \"Upper\",\n        \"Mixed\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avatax-rest-address-validation-info-schema.json
tags:
- Taxes
title: AddressValidationInfo
---
