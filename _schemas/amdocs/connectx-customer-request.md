---
description: CustomerRequest schema from Amdocs API
layout: schema
name: CustomerRequest
properties_list:
- description: ''
  name: customerType
  type: string
- description: ''
  name: firstName
  type: string
- description: ''
  name: lastName
  type: string
- description: ''
  name: companyName
  type: string
- description: ''
  name: email
  type: string
- description: ''
  name: phone
  type: string
- description: ''
  name: address
  type: object
provider_name: Amdocs
provider_slug: amdocs
schema_file: json-schema/connectx-customer-request-schema.json
slug: connectx-customer-request
source_filename: connectx-customer-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amdocs/refs/heads/main/json-schema/connectx-customer-request-schema.json\",\n  \"title\": \"CustomerRequest\",\n  \"description\": \"CustomerRequest schema from Amdocs API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"customerType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Individual\",\n        \"Business\",\n        \"Government\"\n      ]\n    },\n    \"firstName\": {\n      \"type\": \"string\"\n    },\n    \"lastName\": {\n      \"type\": \"string\"\n    },\n    \"companyName\": {\n      \"type\": \"string\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\"\n    },\n    \"phone\": {\n      \"type\": \"string\"\n    },\n    \"address\": {\n      \"$ref\": \"#/components/schemas/Address\"\n    }\n  },\n  \"required\": [\n    \"customerType\",\n    \"email\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amdocs/refs/heads/main/json-schema/connectx-customer-request-schema.json
tags:
- Telecom
- BSS
- OSS
- Billing
- Customer Management
- MVNO
- 5G
- SaaS
title: CustomerRequest
---
