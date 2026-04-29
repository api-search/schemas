---
description: ''
layout: schema
name: Detail10
properties_list:
- description: ''
  name: success
  type: boolean
- description: ''
  name: links
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-detail10-schema.json
slug: salesforce-detail10
source_filename: salesforce-detail10-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"success\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"links\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"giftcommitment\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"href\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            },\n            \"id\": {\n              \"type\": \"string\",\n              \"example\": \"abc123\"\n            }\n          },\n          \"required\": [\n            \"href\",\n            \"id\"\n          ]\n        },\n        \"giftcommitmentschedule\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"href\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            },\n            \"id\": {\n              \"type\": \"string\",\n              \"example\": \"abc123\"\n            }\n    \
  \      },\n          \"required\": [\n            \"href\",\n            \"id\"\n          ]\n        },\n        \"giftdefaultdesignation\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"href\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              },\n              \"id\": {\n                \"type\": \"string\",\n                \"example\": \"abc123\"\n              }\n            },\n            \"required\": [\n              \"href\",\n              \"id\"\n            ]\n          }\n        },\n        \"account\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"href\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            },\n            \"id\": {\n              \"type\": \"string\",\n              \"\
  example\": \"abc123\"\n            }\n          },\n          \"required\": [\n            \"href\",\n            \"id\"\n          ]\n        }\n      },\n      \"required\": [\n        \"giftcommitment\",\n        \"giftcommitmentschedule\",\n        \"giftdefaultdesignation\",\n        \"account\"\n      ]\n    }\n  },\n  \"required\": [\n    \"success\",\n    \"links\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Detail10\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-detail10-schema.json
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
title: Detail10
---
