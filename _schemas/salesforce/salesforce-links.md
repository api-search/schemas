---
description: ''
layout: schema
name: Links
properties_list:
- description: ''
  name: account
  type: object
- description: ''
  name: gifttransaction
  type: object
- description: ''
  name: giftcommitment
  type: object
- description: ''
  name: paymentinstrument
  type: object
- description: ''
  name: gifttransactiondesignation
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-links-schema.json
slug: salesforce-links
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"account\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"href\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"id\": {\n          \"type\": \"string\",\n          \"example\": \"abc123\"\n        }\n      },\n      \"required\": [\n        \"href\",\n        \"id\"\n      ]\n    },\n    \"gifttransaction\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"href\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"id\": {\n          \"type\": \"string\",\n          \"example\": \"abc123\"\n        }\n      },\n      \"required\": [\n        \"href\",\n        \"id\"\n      ]\n    },\n    \"giftcommitment\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"href\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"id\"\
  : {\n          \"type\": \"string\",\n          \"example\": \"abc123\"\n        }\n      },\n      \"required\": [\n        \"href\",\n        \"id\"\n      ]\n    },\n    \"paymentinstrument\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"href\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"id\": {\n          \"type\": \"string\",\n          \"example\": \"abc123\"\n        }\n      },\n      \"required\": [\n        \"href\",\n        \"id\"\n      ]\n    },\n    \"gifttransactiondesignation\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"href\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"id\": {\n            \"type\": \"string\",\n            \"example\": \"abc123\"\n          }\n        },\n        \"required\": [\n\
  \          \"href\",\n          \"id\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"account\",\n    \"gifttransaction\",\n    \"giftcommitment\",\n    \"paymentinstrument\",\n    \"gifttransactiondesignation\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Links\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-links-schema.json
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
title: Links
---
