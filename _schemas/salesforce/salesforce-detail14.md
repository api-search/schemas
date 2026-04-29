---
description: ''
layout: schema
name: Detail14
properties_list:
- description: ''
  name: success
  type: boolean
- description: ''
  name: errors
  type: object
- description: ''
  name: links
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-detail14-schema.json
slug: salesforce-detail14
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"success\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"errors\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"field\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"message\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"field\",\n        \"message\"\n      ]\n    },\n    \"links\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"giftcommitment\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"href\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            },\n            \"id\": {\n              \"type\": \"string\",\n              \"example\": \"abc123\"\n            }\n          },\n          \"required\": [\n            \"href\",\n     \
  \       \"id\"\n          ]\n        },\n        \"paymentinstrument\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"href\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            },\n            \"id\": {\n              \"type\": \"string\",\n              \"example\": \"abc123\"\n            }\n          },\n          \"required\": [\n            \"href\",\n            \"id\"\n          ]\n        }\n      },\n      \"required\": [\n        \"giftcommitment\",\n        \"paymentinstrument\"\n      ]\n    }\n  },\n  \"required\": [\n    \"success\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Detail14\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-detail14-schema.json
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
title: Detail14
---
