---
description: ''
layout: schema
name: Company13
properties_list:
- description: ''
  name: division
  type: string
- description: ''
  name: id
  type: integer
- description: ''
  name: name
  type: string
- description: ''
  name: descriptionList
  type: array
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
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-company13-schema.json
slug: zoominfo-company13
source_filename: zoominfo-company13-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"division\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"id\": {\n      \"type\": \"integer\",\n      \"example\": 500123\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"Acme Corporation\"\n    },\n    \"descriptionList\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"description\": {\n            \"type\": \"string\",\n            \"example\": \"Enterprise software company\"\n          }\n        },\n        \"required\": [\n          \"description\"\n        ]\n      }\n    },\n    \"phone\": {\n      \"type\": \"string\",\n      \"example\": \"+1-555-555-1234\"\n    },\n    \"fax\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"street\": {\n      \"type\": \"string\",\n      \"example\"\
  : \"example_value\"\n    },\n    \"city\": {\n      \"type\": \"string\",\n      \"example\": \"San Francisco\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"example\": \"CA\"\n    },\n    \"zipCode\": {\n      \"type\": \"string\",\n      \"example\": \"94105\"\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"example\": \"US\"\n    }\n  },\n  \"required\": [\n    \"division\",\n    \"id\",\n    \"name\",\n    \"descriptionList\",\n    \"phone\",\n    \"fax\",\n    \"street\",\n    \"city\",\n    \"state\",\n    \"zipCode\",\n    \"country\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Company13\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-company13-schema.json
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
title: Company13
---
