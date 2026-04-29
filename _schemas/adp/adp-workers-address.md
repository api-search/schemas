---
description: ''
layout: schema
name: Address
properties_list:
- description: ''
  name: lineOne
  type: string
- description: ''
  name: lineTwo
  type: string
- description: ''
  name: cityName
  type: string
- description: ''
  name: countrySubdivisionLevel1
  type: object
- description: ''
  name: postalCode
  type: string
- description: ''
  name: countryCode
  type: string
provider_name: ADP
provider_slug: adp
schema_file: json-schema/adp-workers-address-schema.json
slug: adp-workers-address
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Address\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"lineOne\": {\n      \"type\": \"string\"\n    },\n    \"lineTwo\": {\n      \"type\": \"string\"\n    },\n    \"cityName\": {\n      \"type\": \"string\"\n    },\n    \"countrySubdivisionLevel1\": {\n      \"type\": \"object\"\n    },\n    \"postalCode\": {\n      \"type\": \"string\"\n    },\n    \"countryCode\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adp/refs/heads/main/json-schema/adp-workers-address-schema.json
tags:
- Benefits
- HCM
- HR
- Payroll
- Workforce
title: Address
---
