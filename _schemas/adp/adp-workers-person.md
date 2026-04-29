---
description: ''
layout: schema
name: Person
properties_list:
- description: ''
  name: legalName
  type: object
- description: ''
  name: birthDate
  type: string
- description: ''
  name: genderCode
  type: object
- description: ''
  name: maritalStatusCode
  type: object
- description: ''
  name: communication
  type: object
provider_name: ADP
provider_slug: adp
schema_file: json-schema/adp-workers-person-schema.json
slug: adp-workers-person
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Person\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"legalName\": {\n      \"type\": \"object\"\n    },\n    \"birthDate\": {\n      \"type\": \"string\"\n    },\n    \"genderCode\": {\n      \"type\": \"object\"\n    },\n    \"maritalStatusCode\": {\n      \"type\": \"object\"\n    },\n    \"communication\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adp/refs/heads/main/json-schema/adp-workers-person-schema.json
tags:
- Benefits
- HCM
- HR
- Payroll
- Workforce
title: Person
---
