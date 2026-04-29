---
description: ''
layout: schema
name: Datum11
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: category
  type: string
- description: ''
  name: topic
  type: string
- description: ''
  name: signalScore
  type: integer
- description: ''
  name: audienceStrength
  type: string
- description: ''
  name: newSignal
  type: boolean
- description: ''
  name: signalDate
  type: string
- description: ''
  name: trend
  type: integer
- description: ''
  name: recommendedContacts
  type: array
- description: ''
  name: company
  type: object
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-datum11-schema.json
slug: zoominfo-datum11
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"topic\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"signalScore\": {\n      \"type\": \"integer\",\n      \"example\": 85\n    },\n    \"audienceStrength\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"newSignal\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"signalDate\": {\n      \"type\": \"string\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"trend\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    },\n    \"recommendedContacts\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\"\
  : {\n            \"type\": \"integer\",\n            \"example\": 500123\n          },\n          \"firstName\": {\n            \"type\": \"string\",\n            \"example\": \"Acme Corporation\"\n          },\n          \"lastName\": {\n            \"type\": \"string\",\n            \"example\": \"Acme Corporation\"\n          },\n          \"jobTitle\": {\n            \"type\": \"string\",\n            \"example\": \"Vice President of Sales\"\n          },\n          \"jobFunction\": {\n            \"type\": \"array\",\n            \"description\": \"\",\n            \"example\": [],\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"name\": {\n                  \"type\": \"string\",\n                  \"example\": \"Acme Corporation\"\n                },\n                \"department\": {\n                  \"type\": \"string\",\n                  \"example\": \"example_value\"\n                }\n              },\n  \
  \            \"required\": [\n                \"name\",\n                \"department\"\n              ]\n            }\n          }\n        },\n        \"required\": [\n          \"id\",\n          \"firstName\",\n          \"lastName\",\n          \"jobTitle\",\n          \"jobFunction\"\n        ]\n      }\n    },\n    \"company\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\",\n          \"example\": 500123\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"example\": \"Acme Corporation\"\n        },\n        \"website\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"hasOtherTopicConsumption\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        }\n      },\n      \"required\": [\n        \"id\",\n        \"name\",\n        \"website\",\n        \"hasOtherTopicConsumption\"\n      ]\n    }\n  },\n  \"required\": [\n \
  \   \"id\",\n    \"category\",\n    \"topic\",\n    \"signalScore\",\n    \"audienceStrength\",\n    \"newSignal\",\n    \"signalDate\",\n    \"trend\",\n    \"recommendedContacts\",\n    \"company\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Datum11\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-datum11-schema.json
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
title: Datum11
---
