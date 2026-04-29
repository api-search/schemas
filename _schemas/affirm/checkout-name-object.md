---
description: A person's name split into first and last components.
layout: schema
name: NameObject
properties_list:
- description: First name.
  name: first
  type: string
- description: Last name.
  name: last
  type: string
- description: Full name as a single string.
  name: full
  type: string
provider_name: affirm
provider_slug: affirm
schema_file: json-schema/checkout-name-object-schema.json
slug: checkout-name-object
source_filename: checkout-name-object-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/affirm/refs/heads/main/json-schema/checkout-name-object-schema.json\",\n  \"title\": \"NameObject\",\n  \"description\": \"A person's name split into first and last components.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"first\": {\n      \"type\": \"string\",\n      \"description\": \"First name.\",\n      \"example\": \"example_value\"\n    },\n    \"last\": {\n      \"type\": \"string\",\n      \"description\": \"Last name.\",\n      \"example\": \"example_value\"\n    },\n    \"full\": {\n      \"type\": \"string\",\n      \"description\": \"Full name as a single string.\",\n      \"example\": \"example_value\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/affirm/refs/heads/main/json-schema/checkout-name-object-schema.json
tags: []
title: NameObject
---
