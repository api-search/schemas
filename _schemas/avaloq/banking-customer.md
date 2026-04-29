---
description: Banking customer record
layout: schema
name: Customer
properties_list:
- description: Customer ID
  name: id
  type: string
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
  name: status
  type: string
- description: ''
  name: kycStatus
  type: string
- description: ''
  name: clientSince
  type: string
- description: ''
  name: residenceCountry
  type: string
- description: ''
  name: taxResidency
  type: string
provider_name: Avaloq
provider_slug: avaloq
schema_file: json-schema/banking-customer-schema.json
slug: banking-customer
source_filename: banking-customer-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avaloq/refs/heads/main/json-schema/banking-customer-schema.json\",\n  \"title\": \"Customer\",\n  \"description\": \"Banking customer record\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Customer ID\",\n      \"example\": \"CUST-001234\"\n    },\n    \"firstName\": {\n      \"type\": \"string\",\n      \"example\": \"Jane\"\n    },\n    \"lastName\": {\n      \"type\": \"string\",\n      \"example\": \"Smith\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"example\": \"jane.smith@example.com\"\n    },\n    \"phone\": {\n      \"type\": \"string\",\n      \"example\": \"+41791234567\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ACTIVE\",\n        \"INACTIVE\",\n        \"SUSPENDED\"\n  \
  \    ],\n      \"example\": \"ACTIVE\"\n    },\n    \"kycStatus\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"PENDING\",\n        \"APPROVED\",\n        \"REJECTED\",\n        \"REQUIRES_REVIEW\"\n      ],\n      \"example\": \"APPROVED\"\n    },\n    \"clientSince\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"example\": \"2020-01-15\"\n    },\n    \"residenceCountry\": {\n      \"type\": \"string\",\n      \"example\": \"CH\"\n    },\n    \"taxResidency\": {\n      \"type\": \"string\",\n      \"example\": \"CH\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avaloq/refs/heads/main/json-schema/banking-customer-schema.json
tags:
- Banking
- Digital Banking
- Financial Services
- Fintech
- Payments
- Wealth Management
title: Customer
---
