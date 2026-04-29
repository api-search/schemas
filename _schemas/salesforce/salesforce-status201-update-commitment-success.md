---
description: ''
layout: schema
name: Status201-UpdateCommitmentSuccess
properties_list:
- description: ''
  name: successes
  type: integer
- description: ''
  name: failures
  type: integer
- description: ''
  name: notProcessed
  type: integer
- description: ''
  name: details
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-status201-update-commitment-success-schema.json
slug: salesforce-status201-update-commitment-success
source_filename: salesforce-status201-update-commitment-success-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"successes\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"failures\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"notProcessed\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"details\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"success\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"links\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"giftcommitment\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"href\": {\n                    \"type\": \"string\",\n                    \"example\": \"example_value\"\n                  },\n                  \"id\": {\n                    \"\
  type\": \"string\",\n                    \"example\": \"abc123\"\n                  }\n                },\n                \"required\": [\n                  \"href\",\n                  \"id\"\n                ]\n              },\n              \"paymentinstrument\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"href\": {\n                    \"type\": \"string\",\n                    \"example\": \"example_value\"\n                  },\n                  \"id\": {\n                    \"type\": \"string\",\n                    \"example\": \"abc123\"\n                  }\n                },\n                \"required\": [\n                  \"href\",\n                  \"id\"\n                ]\n              }\n            },\n            \"required\": [\n              \"giftcommitment\",\n              \"paymentinstrument\"\n            ]\n          }\n        },\n        \"required\": [\n          \"success\",\n          \"links\"\
  \n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"successes\",\n    \"failures\",\n    \"notProcessed\",\n    \"details\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Status201-UpdateCommitmentSuccess\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-status201-update-commitment-success-schema.json
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
title: Status201-UpdateCommitmentSuccess
---
