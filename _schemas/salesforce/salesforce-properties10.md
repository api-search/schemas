---
description: ''
layout: schema
name: Properties10
properties_list:
- description: ''
  name: message
  type: object
- description: ''
  name: statusCode
  type: object
- description: ''
  name: extendedDetails
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-properties10-schema.json
slug: salesforce-properties10
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"message\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"type\"\n      ]\n    },\n    \"statusCode\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"type\"\n      ]\n    },\n    \"extendedDetails\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"items\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"type\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            },\n            \"properties\": {\n        \
  \      \"type\": \"object\",\n              \"example\": \"example_value\"\n            }\n          },\n          \"required\": [\n            \"type\",\n            \"properties\"\n          ]\n        }\n      },\n      \"required\": [\n        \"type\",\n        \"items\"\n      ]\n    }\n  },\n  \"required\": [\n    \"message\",\n    \"statusCode\",\n    \"extendedDetails\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Properties10\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-properties10-schema.json
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
title: Properties10
---
