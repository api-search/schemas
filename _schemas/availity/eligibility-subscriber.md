---
description: Subscriber schema from Availity API
layout: schema
name: Subscriber
properties_list:
- description: Insurance member ID
  name: memberId
  type: string
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
- description: Social Security Number (last 4 or full)
  name: ssn
  type: string
- description: ''
  name: groupNumber
  type: string
provider_name: availity
provider_slug: availity
schema_file: json-schema/eligibility-subscriber-schema.json
slug: eligibility-subscriber
source_filename: eligibility-subscriber-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/json-schema/eligibility-subscriber-schema.json\",\n  \"title\": \"Subscriber\",\n  \"description\": \"Subscriber schema from Availity API\",\n  \"type\": \"object\",\n  \"required\": [\n    \"memberId\"\n  ],\n  \"properties\": {\n    \"memberId\": {\n      \"type\": \"string\",\n      \"description\": \"Insurance member ID\"\n    },\n    \"firstName\": {\n      \"type\": \"string\"\n    },\n    \"lastName\": {\n      \"type\": \"string\"\n    },\n    \"dateOfBirth\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"gender\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"M\",\n        \"F\",\n        \"U\"\n      ]\n    },\n    \"ssn\": {\n      \"type\": \"string\",\n      \"description\": \"Social Security Number (last 4 or full)\"\n    },\n    \"groupNumber\": {\n      \"type\"\
  : \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/json-schema/eligibility-subscriber-schema.json
tags: []
title: Subscriber
---
