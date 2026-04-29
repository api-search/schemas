---
description: ''
layout: schema
name: Section1
properties_list:
- description: ''
  name: collapsible
  type: boolean
- description: ''
  name: columns
  type: integer
- description: ''
  name: heading
  type: string
- description: ''
  name: id
  type: string
- description: ''
  name: layoutRows
  type: array
- description: ''
  name: rows
  type: integer
- description: ''
  name: useHeading
  type: boolean
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-section1-schema.json
slug: salesforce-section1
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"collapsible\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"columns\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"heading\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"example\": \"abc123\"\n    },\n    \"layoutRows\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"layoutItems\": {\n            \"type\": \"array\",\n            \"description\": \"\",\n            \"example\": [],\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"editableForNew\": {\n                  \"type\": \"boolean\",\n                  \"example\": true\n                },\n                \"editableForUpdate\": {\n   \
  \               \"type\": \"boolean\",\n                  \"example\": true\n                },\n                \"label\": {\n                  \"type\": \"string\",\n                  \"example\": \"Example Title\"\n                },\n                \"layoutComponents\": {\n                  \"type\": \"array\",\n                  \"description\": \"\",\n                  \"example\": [],\n                  \"items\": {\n                    \"type\": \"object\"\n                  }\n                },\n                \"lookupIdApiName\": {\n                  \"type\": \"['string', 'null']\",\n                  \"example\": \"example_value\"\n                },\n                \"required\": {\n                  \"type\": \"boolean\",\n                  \"example\": true\n                },\n                \"sortable\": {\n                  \"type\": \"boolean\",\n                  \"example\": true\n                }\n              },\n              \"required\": [\n            \
  \    \"editableForNew\",\n                \"editableForUpdate\",\n                \"label\",\n                \"layoutComponents\",\n                \"lookupIdApiName\",\n                \"required\",\n                \"sortable\"\n              ]\n            }\n          }\n        },\n        \"required\": [\n          \"layoutItems\"\n        ]\n      }\n    },\n    \"rows\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"useHeading\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    }\n  },\n  \"required\": [\n    \"collapsible\",\n    \"columns\",\n    \"heading\",\n    \"id\",\n    \"layoutRows\",\n    \"rows\",\n    \"useHeading\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Section1\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-section1-schema.json
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
title: Section1
---
