---
description: Request to create a new customer
layout: schema
name: CreateCustomerRequest
properties_list:
- description: ''
  name: firstName
  type: string
- description: ''
  name: lastName
  type: string
- description: ''
  name: email
  type: string
- description: ''
  name: phone
  type: string
- description: ''
  name: residenceCountry
  type: string
- description: ''
  name: dateOfBirth
  type: string
provider_name: Avaloq
provider_slug: avaloq
schema_file: json-schema/banking-create-customer-request-schema.json
slug: banking-create-customer-request
source_filename: banking-create-customer-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avaloq/refs/heads/main/json-schema/banking-create-customer-request-schema.json\",\n  \"title\": \"CreateCustomerRequest\",\n  \"description\": \"Request to create a new customer\",\n  \"type\": \"object\",\n  \"required\": [\n    \"firstName\",\n    \"lastName\",\n    \"email\"\n  ],\n  \"properties\": {\n    \"firstName\": {\n      \"type\": \"string\",\n      \"example\": \"Jane\"\n    },\n    \"lastName\": {\n      \"type\": \"string\",\n      \"example\": \"Smith\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"example\": \"jane.smith@example.com\"\n    },\n    \"phone\": {\n      \"type\": \"string\",\n      \"example\": \"+41791234567\"\n    },\n    \"residenceCountry\": {\n      \"type\": \"string\",\n      \"example\": \"CH\"\n    },\n    \"dateOfBirth\": {\n      \"type\": \"string\",\n   \
  \   \"format\": \"date\",\n      \"example\": \"1980-06-15\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avaloq/refs/heads/main/json-schema/banking-create-customer-request-schema.json
tags:
- Banking
- Digital Banking
- Financial Services
- Fintech
- Payments
- Wealth Management
title: CreateCustomerRequest
---
