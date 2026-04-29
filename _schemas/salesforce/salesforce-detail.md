---
description: ''
layout: schema
name: Detail
properties_list:
- description: ''
  name: success
  type: boolean
- description: ''
  name: links
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-detail-schema.json
slug: salesforce-detail
source_filename: salesforce-detail-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"success\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"links\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"account\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"href\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            },\n            \"id\": {\n              \"type\": \"string\",\n              \"example\": \"abc123\"\n            }\n          },\n          \"required\": [\n            \"href\",\n            \"id\"\n          ]\n        },\n        \"gifttransaction\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"href\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            },\n            \"id\": {\n              \"type\": \"string\",\n              \"example\": \"abc123\"\n            }\n          },\n    \
  \      \"required\": [\n            \"href\",\n            \"id\"\n          ]\n        },\n        \"giftcommitment\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"href\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            },\n            \"id\": {\n              \"type\": \"string\",\n              \"example\": \"abc123\"\n            }\n          },\n          \"required\": [\n            \"href\",\n            \"id\"\n          ]\n        },\n        \"paymentinstrument\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"href\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            },\n            \"id\": {\n              \"type\": \"string\",\n              \"example\": \"abc123\"\n            }\n          },\n          \"required\": [\n            \"href\",\n            \"id\"\n          ]\n        },\n        \"gifttransactiondesignation\"\
  : {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"href\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              },\n              \"id\": {\n                \"type\": \"string\",\n                \"example\": \"abc123\"\n              }\n            },\n            \"required\": [\n              \"href\",\n              \"id\"\n            ]\n          }\n        }\n      },\n      \"required\": [\n        \"account\",\n        \"gifttransaction\",\n        \"giftcommitment\",\n        \"paymentinstrument\",\n        \"gifttransactiondesignation\"\n      ]\n    }\n  },\n  \"required\": [\n    \"success\",\n    \"links\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Detail\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-detail-schema.json
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
title: Detail
---
