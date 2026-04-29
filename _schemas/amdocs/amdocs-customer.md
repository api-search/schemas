---
description: JSON Schema for an Amdocs BSS telecom customer account.
layout: schema
name: Amdocs Customer
properties_list:
- description: Unique customer identifier
  name: customerId
  type: string
- description: Classification of the customer
  name: customerType
  type: string
- description: ''
  name: status
  type: string
- description: Customer-facing account number
  name: accountNumber
  type: string
- description: ''
  name: firstName
  type: string
- description: ''
  name: lastName
  type: string
- description: Company name for Business/Government customers
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
  name: subscriptions
  type: array
- description: ''
  name: createdAt
  type: string
- description: ''
  name: updatedAt
  type: string
provider_name: Amdocs
provider_slug: amdocs
schema_file: json-schema/amdocs-customer-schema.json
slug: amdocs-customer
source_filename: amdocs-customer-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amdocs/refs/heads/main/json-schema/amdocs-customer-schema.json\",\n  \"title\": \"Amdocs Customer\",\n  \"description\": \"JSON Schema for an Amdocs BSS telecom customer account.\",\n  \"type\": \"object\",\n  \"required\": [\"customerId\", \"customerType\", \"status\"],\n  \"properties\": {\n    \"customerId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique customer identifier\"\n    },\n    \"customerType\": {\n      \"type\": \"string\",\n      \"enum\": [\"Individual\", \"Business\", \"Government\"],\n      \"description\": \"Classification of the customer\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"Active\", \"Inactive\", \"Suspended\", \"Terminated\"]\n    },\n    \"accountNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Customer-facing account number\"\n    },\n    \"firstName\"\
  : {\n      \"type\": \"string\"\n    },\n    \"lastName\": {\n      \"type\": \"string\"\n    },\n    \"companyName\": {\n      \"type\": \"string\",\n      \"description\": \"Company name for Business/Government customers\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\"\n    },\n    \"phone\": {\n      \"type\": \"string\"\n    },\n    \"address\": {\n      \"$ref\": \"#/$defs/Address\"\n    },\n    \"billingAddress\": {\n      \"$ref\": \"#/$defs/Address\"\n    },\n    \"subscriptions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Subscription\"\n      }\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  },\n  \"$defs\": {\n    \"Address\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"street\": {\"type\": \"string\"},\n        \"city\": {\"type\": \"\
  string\"},\n        \"state\": {\"type\": \"string\"},\n        \"postalCode\": {\"type\": \"string\"},\n        \"country\": {\"type\": \"string\"}\n      }\n    },\n    \"Subscription\": {\n      \"type\": \"object\",\n      \"required\": [\"subscriptionId\", \"productId\", \"status\"],\n      \"properties\": {\n        \"subscriptionId\": {\"type\": \"string\"},\n        \"productId\": {\"type\": \"string\"},\n        \"productName\": {\"type\": \"string\"},\n        \"status\": {\n          \"type\": \"string\",\n          \"enum\": [\"Active\", \"Suspended\", \"Cancelled\", \"Pending\"]\n        },\n        \"startDate\": {\"type\": \"string\", \"format\": \"date\"},\n        \"endDate\": {\"type\": \"string\", \"format\": \"date\"},\n        \"monthlyCharge\": {\"type\": \"number\", \"minimum\": 0},\n        \"currency\": {\"type\": \"string\"}\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amdocs/refs/heads/main/json-schema/amdocs-customer-schema.json
tags:
- Telecom
- BSS
- OSS
- Billing
- Customer Management
- MVNO
- 5G
- SaaS
title: Amdocs Customer
---
