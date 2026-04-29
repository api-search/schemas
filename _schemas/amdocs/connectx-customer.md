---
description: Customer schema from Amdocs API
layout: schema
name: Customer
properties_list:
- description: ''
  name: customerId
  type: string
- description: ''
  name: customerType
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: accountNumber
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
- description: ''
  name: billingAddress
  type: object
- description: ''
  name: createdAt
  type: string
- description: ''
  name: updatedAt
  type: string
provider_name: Amdocs
provider_slug: amdocs
schema_file: json-schema/connectx-customer-schema.json
slug: connectx-customer
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amdocs/refs/heads/main/json-schema/connectx-customer-schema.json\",\n  \"title\": \"Customer\",\n  \"description\": \"Customer schema from Amdocs API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"customerId\": {\n      \"type\": \"string\"\n    },\n    \"customerType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Individual\",\n        \"Business\",\n        \"Government\"\n      ]\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Active\",\n        \"Inactive\",\n        \"Suspended\",\n        \"Terminated\"\n      ]\n    },\n    \"accountNumber\": {\n      \"type\": \"string\"\n    },\n    \"firstName\": {\n      \"type\": \"string\"\n    },\n    \"lastName\": {\n      \"type\": \"string\"\n    },\n    \"companyName\": {\n      \"type\": \"string\"\n    },\n    \"email\": {\n    \
  \  \"type\": \"string\",\n      \"format\": \"email\"\n    },\n    \"phone\": {\n      \"type\": \"string\"\n    },\n    \"address\": {\n      \"$ref\": \"#/components/schemas/Address\"\n    },\n    \"billingAddress\": {\n      \"$ref\": \"#/components/schemas/Address\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amdocs/refs/heads/main/json-schema/connectx-customer-schema.json
tags:
- Telecom
- BSS
- OSS
- Billing
- Customer Management
- MVNO
- 5G
- SaaS
title: Customer
---
