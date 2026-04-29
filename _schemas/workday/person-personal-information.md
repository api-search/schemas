---
description: ''
layout: schema
name: PersonalInformation
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: dateOfBirth
  type: string
- description: ''
  name: disability
  type: array
provider_name: Workday
provider_slug: workday
schema_file: json-schema/person-personal-information-schema.json
slug: person-personal-information
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PersonalInformation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"dateOfBirth\": {\n      \"type\": \"string\"\n    },\n    \"disability\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/json-schema/person-personal-information-schema.json
tags:
- Cloud Computing
- Enterprise Software
- Financial Management
- HCM
- SaaS
title: PersonalInformation
---
