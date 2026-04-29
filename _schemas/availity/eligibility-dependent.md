---
description: Dependent schema from Availity API
layout: schema
name: Dependent
properties_list:
- description: ''
  name: firstName
  type: string
- description: ''
  name: lastName
  type: string
- description: ''
  name: dateOfBirth
  type: string
- description: ''
  name: gender
  type: string
- description: ''
  name: relationship
  type: string
provider_name: availity
provider_slug: availity
schema_file: json-schema/eligibility-dependent-schema.json
slug: eligibility-dependent
source_filename: eligibility-dependent-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/json-schema/eligibility-dependent-schema.json\",\n  \"title\": \"Dependent\",\n  \"description\": \"Dependent schema from Availity API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"firstName\": {\n      \"type\": \"string\"\n    },\n    \"lastName\": {\n      \"type\": \"string\"\n    },\n    \"dateOfBirth\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"gender\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"M\",\n        \"F\",\n        \"U\"\n      ]\n    },\n    \"relationship\": {\n      \"type\": \"string\",\n      \"enum\": [\n        1,\n        19,\n        20,\n        21,\n        39,\n        40,\n        \"G8\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/json-schema/eligibility-dependent-schema.json
tags: []
title: Dependent
---
