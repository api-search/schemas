---
description: ''
layout: schema
name: Candidate
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: descriptor
  type: string
- description: The full name of the candidate.
  name: name
  type: string
- description: ''
  name: email
  type: string
- description: ''
  name: phone
  type: string
- description: ''
  name: attachments
  type: array
provider_name: Workday
provider_slug: workday
schema_file: json-schema/recruiting-candidate-schema.json
slug: recruiting-candidate
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Candidate\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"descriptor\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The full name of the candidate.\"\n    },\n    \"email\": {\n      \"type\": \"string\"\n    },\n    \"phone\": {\n      \"type\": \"string\"\n    },\n    \"attachments\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/json-schema/recruiting-candidate-schema.json
tags:
- Cloud Computing
- Enterprise Software
- Financial Management
- HCM
- SaaS
title: Candidate
---
