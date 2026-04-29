---
description: ''
layout: schema
name: Links7
properties_list:
- description: ''
  name: giftcommitment
  type: object
- description: ''
  name: giftcommitmentschedule
  type: object
- description: ''
  name: giftdefaultdesignation
  type: array
- description: ''
  name: gifttransaction
  type: object
- description: ''
  name: paymentinstrument
  type: object
- description: ''
  name: account
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-links7-schema.json
slug: salesforce-links7
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"giftcommitment\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"href\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"id\": {\n          \"type\": \"string\",\n          \"example\": \"abc123\"\n        }\n      },\n      \"required\": [\n        \"href\",\n        \"id\"\n      ]\n    },\n    \"giftcommitmentschedule\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"href\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"id\": {\n          \"type\": \"string\",\n          \"example\": \"abc123\"\n        }\n      },\n      \"required\": [\n        \"href\",\n        \"id\"\n      ]\n    },\n    \"giftdefaultdesignation\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\"\
  : {\n          \"href\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"id\": {\n            \"type\": \"string\",\n            \"example\": \"abc123\"\n          }\n        },\n        \"required\": [\n          \"href\",\n          \"id\"\n        ]\n      }\n    },\n    \"gifttransaction\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"href\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"id\": {\n          \"type\": \"string\",\n          \"example\": \"abc123\"\n        }\n      },\n      \"required\": [\n        \"href\",\n        \"id\"\n      ]\n    },\n    \"paymentinstrument\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"href\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"id\": {\n          \"type\": \"string\",\n          \"example\": \"abc123\"\n        }\n     \
  \ },\n      \"required\": [\n        \"href\",\n        \"id\"\n      ]\n    },\n    \"account\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"href\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"id\": {\n          \"type\": \"string\",\n          \"example\": \"abc123\"\n        }\n      },\n      \"required\": [\n        \"href\",\n        \"id\"\n      ]\n    }\n  },\n  \"required\": [\n    \"giftcommitment\",\n    \"giftcommitmentschedule\",\n    \"giftdefaultdesignation\",\n    \"gifttransaction\",\n    \"paymentinstrument\",\n    \"account\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Links7\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-links7-schema.json
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
title: Links7
---
