---
description: ''
layout: schema
name: Datum8
properties_list:
- description: ''
  name: id
  type: integer
- description: ''
  name: publishedDate
  type: string
- description: ''
  name: originalPublishedDate
  type: string
- description: ''
  name: linkText
  type: string
- description: ''
  name: link
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: topics
  type: array
- description: ''
  name: updateText
  type: string
- description: ''
  name: types
  type: array
- description: ''
  name: contacts
  type: array
- description: ''
  name: company
  type: object
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-datum8-schema.json
slug: zoominfo-datum8
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"example\": 500123\n    },\n    \"publishedDate\": {\n      \"type\": \"string\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"originalPublishedDate\": {\n      \"type\": \"string\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"linkText\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"link\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"example\": \"Enterprise software company\"\n    },\n    \"topics\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"updateText\": {\n      \"type\": \"string\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"types\": {\n      \"type\": \"array\",\n      \"description\"\
  : \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"integer\",\n            \"example\": 500123\n          },\n          \"type\": {\n            \"type\": \"string\",\n            \"example\": \"standard\"\n          }\n        },\n        \"required\": [\n          \"id\",\n          \"type\"\n        ]\n      }\n    },\n    \"contacts\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"company\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\",\n          \"example\": 500123\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"example\": \"Acme Corporation\"\n        }\n      },\n      \"required\": [\n        \"id\",\n        \"name\"\n      ]\n    }\n  },\n  \"required\": [\n    \"id\",\n\
  \    \"publishedDate\",\n    \"originalPublishedDate\",\n    \"linkText\",\n    \"link\",\n    \"description\",\n    \"topics\",\n    \"updateText\",\n    \"types\",\n    \"contacts\",\n    \"company\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Datum8\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-datum8-schema.json
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
title: Datum8
---
