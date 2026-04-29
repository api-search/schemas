---
description: ''
layout: schema
name: CreateUserRequest
properties_list:
- description: User email address
  name: email
  type: string
- description: User mobile number in E.164 format
  name: mobile
  type: string
- description: ''
  name: firstName
  type: string
- description: ''
  name: lastName
  type: string
provider_name: Basiq
provider_slug: basiq
schema_file: json-schema/createuserrequest.json
slug: createuserrequest
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/basiq/refs/heads/main/json-schema/createuserrequest.json\",\n  \"title\": \"CreateUserRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"User email address\"\n    },\n    \"mobile\": {\n      \"type\": \"string\",\n      \"description\": \"User mobile number in E.164 format\"\n    },\n    \"firstName\": {\n      \"type\": \"string\"\n    },\n    \"lastName\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/basiq/refs/heads/main/json-schema/createuserrequest.json
tags:
- Australia
- Banking
- CDR
- Financial Data
- Fintech
- Open Banking
- Transactions
title: CreateUserRequest
---
