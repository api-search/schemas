---
description: ''
layout: schema
name: Phone
properties_list:
- description: ''
  name: phoneId
  type: integer
- description: Phone type
  name: phoneType
  type: string
- description: ''
  name: phoneNumber
  type: string
- description: ''
  name: dateFrom
  type: string
- description: ''
  name: dateTo
  type: string
provider_name: Oracle E-Business Suite
provider_slug: oracle-e-business-suite
schema_file: json-schema/human-resources-phone-schema.json
slug: human-resources-phone
source_filename: human-resources-phone-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Phone\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"phoneId\": {\n      \"type\": \"integer\"\n    },\n    \"phoneType\": {\n      \"type\": \"string\",\n      \"description\": \"Phone type\"\n    },\n    \"phoneNumber\": {\n      \"type\": \"string\"\n    },\n    \"dateFrom\": {\n      \"type\": \"string\"\n    },\n    \"dateTo\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/json-schema/human-resources-phone-schema.json
tags:
- Business Applications
- E-Business Suite
- Enterprise
- ERP
- Oracle
title: Phone
---
