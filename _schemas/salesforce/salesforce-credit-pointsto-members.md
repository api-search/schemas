---
description: ''
layout: schema
name: CreditPointstoMembers
properties_list:
- description: ''
  name: message
  type: '[''string'', ''null'']'
- description: ''
  name: outputParameters
  type: object
- description: ''
  name: simulationDetails
  type: object
- description: ''
  name: status
  type: boolean
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-credit-pointsto-members-schema.json
slug: salesforce-credit-pointsto-members
source_filename: salesforce-credit-pointsto-members-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"message\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"outputParameters\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"outputParameters\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"results\": {\n              \"type\": \"array\",\n              \"description\": \"\",\n              \"example\": [],\n              \"items\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"PointsCredited\": {\n                    \"type\": \"integer\",\n                    \"example\": 10\n                  }\n                },\n                \"required\": [\n                  \"PointsCredited\"\n                ]\n              }\n            }\n          },\n          \"required\": [\n            \"results\"\n          ]\n        }\n      },\n      \"required\": [\n        \"\
  outputParameters\"\n      ]\n    },\n    \"simulationDetails\": {\n      \"type\": \"object\",\n      \"example\": \"example_value\"\n    },\n    \"status\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    }\n  },\n  \"required\": [\n    \"message\",\n    \"outputParameters\",\n    \"simulationDetails\",\n    \"status\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreditPointstoMembers\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-credit-pointsto-members-schema.json
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
title: CreditPointstoMembers
---
