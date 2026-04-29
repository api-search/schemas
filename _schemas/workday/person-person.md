---
description: ''
layout: schema
name: Person
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: descriptor
  type: string
- description: ''
  name: dateOfBirth
  type: string
- description: ''
  name: citizenship
  type: array
provider_name: Workday
provider_slug: workday
schema_file: json-schema/person-person-schema.json
slug: person-person
source_filename: person-person-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Person\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"descriptor\": {\n      \"type\": \"string\"\n    },\n    \"dateOfBirth\": {\n      \"type\": \"string\"\n    },\n    \"citizenship\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/json-schema/person-person-schema.json
tags:
- Cloud Computing
- Enterprise Software
- Financial Management
- HCM
- SaaS
title: Person
---
