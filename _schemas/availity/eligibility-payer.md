---
description: Payer schema from Availity API
layout: schema
name: Payer
properties_list:
- description: Availity payer ID
  name: id
  type: string
- description: ''
  name: name
  type: string
provider_name: availity
provider_slug: availity
schema_file: json-schema/eligibility-payer-schema.json
slug: eligibility-payer
source_filename: eligibility-payer-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/json-schema/eligibility-payer-schema.json\",\n  \"title\": \"Payer\",\n  \"description\": \"Payer schema from Availity API\",\n  \"type\": \"object\",\n  \"required\": [\n    \"id\"\n  ],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Availity payer ID\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/json-schema/eligibility-payer-schema.json
tags: []
title: Payer
---
