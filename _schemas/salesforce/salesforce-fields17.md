---
description: ''
layout: schema
name: Fields17
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: Rating
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-fields17-schema.json
slug: salesforce-fields17
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"Rating\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\",\n    \"Rating\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"\
  Fields17\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-fields17-schema.json
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
title: Fields17
---
