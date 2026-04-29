---
description: ''
layout: schema
name: Data35
properties_list:
- description: ''
  name: phone
  type: string
- description: ''
  name: fax
  type: string
- description: ''
  name: street
  type: string
- description: ''
  name: city
  type: string
- description: ''
  name: state
  type: string
- description: ''
  name: zipCode
  type: string
- description: ''
  name: country
  type: string
- description: ''
  name: company
  type: object
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-data35-schema.json
slug: zoominfo-data35
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"phone\": {\n      \"type\": \"string\",\n      \"example\": \"+1-555-555-1234\"\n    },\n    \"fax\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"street\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"city\": {\n      \"type\": \"string\",\n      \"example\": \"San Francisco\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"example\": \"CA\"\n    },\n    \"zipCode\": {\n      \"type\": \"string\",\n      \"example\": \"94105\"\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"example\": \"US\"\n    },\n    \"company\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\",\n          \"example\": 500123\n        },\n        \"addressStatus\": {\n          \"type\": \"string\",\n          \"example\": \"123 Main Street\"\n        },\n        \"subUnitType\":\
  \ {\n          \"type\": \"string\",\n          \"example\": \"standard\"\n        },\n        \"locationName\": {\n          \"type\": \"string\",\n          \"example\": \"Acme Corporation\"\n        },\n        \"locationEmployeeCount\": {\n          \"type\": \"integer\",\n          \"example\": 250\n        }\n      },\n      \"required\": [\n        \"id\",\n        \"addressStatus\",\n        \"subUnitType\",\n        \"locationName\",\n        \"locationEmployeeCount\"\n      ]\n    }\n  },\n  \"required\": [\n    \"phone\",\n    \"fax\",\n    \"street\",\n    \"city\",\n    \"state\",\n    \"zipCode\",\n    \"country\",\n    \"company\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Data35\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-data35-schema.json
tags:
- B2B
- B2B Data
- Company Data
- Contact Database
- Contacts
- Data
- Lead Generation
- Marketing Intelligence
- Sales Intelligence
title: Data35
---
