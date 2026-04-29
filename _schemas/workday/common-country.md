---
description: ''
layout: schema
name: Country
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: descriptor
  type: string
- description: The ISO 3166-1 alpha-3 country code.
  name: countryCode
  type: string
- description: The ISO 3166-1 alpha-2 country code.
  name: alpha2Code
  type: string
- description: ''
  name: name
  type: string
provider_name: Workday
provider_slug: workday
schema_file: json-schema/common-country-schema.json
slug: common-country
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Country\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"descriptor\": {\n      \"type\": \"string\"\n    },\n    \"countryCode\": {\n      \"type\": \"string\",\n      \"description\": \"The ISO 3166-1 alpha-3 country code.\"\n    },\n    \"alpha2Code\": {\n      \"type\": \"string\",\n      \"description\": \"The ISO 3166-1 alpha-2 country code.\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/json-schema/common-country-schema.json
tags:
- Cloud Computing
- Enterprise Software
- Financial Management
- HCM
- SaaS
title: Country
---
