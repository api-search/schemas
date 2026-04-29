---
description: ''
layout: schema
name: VisaInfo
properties_list:
- description: Destination country code
  name: destination
  type: string
- description: Passport country code
  name: passport
  type: string
- description: ''
  name: requirement
  type: string
- description: Maximum stay in days
  name: maxStay
  type: integer
- description: ''
  name: notes
  type: string
provider_name: Basetrip
provider_slug: basetrip
schema_file: json-schema/visainfo.json
slug: visainfo
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/basetrip/refs/heads/main/json-schema/visainfo.json\",\n  \"title\": \"VisaInfo\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"destination\": {\n      \"type\": \"string\",\n      \"description\": \"Destination country code\"\n    },\n    \"passport\": {\n      \"type\": \"string\",\n      \"description\": \"Passport country code\"\n    },\n    \"requirement\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Visa Free\",\n        \"Visa on Arrival\",\n        \"e-Visa\",\n        \"Visa Required\",\n        \"No Admission\"\n      ]\n    },\n    \"maxStay\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum stay in days\"\n    },\n    \"notes\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/basetrip/refs/heads/main/json-schema/visainfo.json
tags:
- Cities
- Countries
- Health
- Safety
- Travel
- Visa
title: VisaInfo
---
