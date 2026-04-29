---
description: ''
layout: schema
name: User
properties_list:
- description: Basiq user ID
  name: id
  type: string
- description: ''
  name: email
  type: string
- description: ''
  name: mobile
  type: string
- description: ''
  name: firstName
  type: string
- description: ''
  name: lastName
  type: string
- description: ''
  name: createdDate
  type: string
provider_name: Basiq
provider_slug: basiq
schema_file: json-schema/user.json
slug: user
source_filename: user.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/basiq/refs/heads/main/json-schema/user.json\",\n  \"title\": \"User\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Basiq user ID\"\n    },\n    \"email\": {\n      \"type\": \"string\"\n    },\n    \"mobile\": {\n      \"type\": \"string\"\n    },\n    \"firstName\": {\n      \"type\": \"string\"\n    },\n    \"lastName\": {\n      \"type\": \"string\"\n    },\n    \"createdDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"email\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/basiq/refs/heads/main/json-schema/user.json
tags:
- Australia
- Banking
- CDR
- Financial Data
- Fintech
- Open Banking
- Transactions
title: User
---
