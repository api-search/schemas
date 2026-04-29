---
description: ''
layout: schema
name: Donor3
properties_list:
- description: ''
  name: donorType
  type: string
- description: ''
  name: organizationName
  type: string
- description: ''
  name: firstName
  type: string
- description: ''
  name: lastName
  type: string
- description: ''
  name: phone
  type: string
- description: ''
  name: email
  type: string
- description: ''
  name: address
  type: array
- description: ''
  name: accountCustomFields
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-donor3-schema.json
slug: salesforce-donor3
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"donorType\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"organizationName\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"firstName\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"lastName\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"phone\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"example\": \"user@example.com\"\n    },\n    \"address\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"addressType\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"street\": {\n            \"type\": \"string\"\
  ,\n            \"example\": \"example_value\"\n          },\n          \"city\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"state\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"postalCode\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"country\": {\n            \"type\": \"string\",\n            \"example\": 42\n          }\n        },\n        \"required\": [\n          \"addressType\",\n          \"street\",\n          \"city\",\n          \"state\",\n          \"postalCode\",\n          \"country\"\n        ]\n      }\n    },\n    \"accountCustomFields\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": 42,\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"fieldName\": {\n            \"type\": \"string\",\n            \"example\"\
  : \"example_value\"\n          },\n          \"fieldValue\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          }\n        },\n        \"required\": [\n          \"fieldName\",\n          \"fieldValue\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"donorType\",\n    \"organizationName\",\n    \"firstName\",\n    \"lastName\",\n    \"phone\",\n    \"email\",\n    \"address\",\n    \"accountCustomFields\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Donor3\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-donor3-schema.json
tags:
- AI
- Analytics
- Cloud
- Commerce
- CRM
- Customer Service
- Enterprise
- Marketing
- Platform
- Sales
title: Donor3
---
