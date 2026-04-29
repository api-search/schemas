---
description: ''
layout: schema
name: OutputParameters2
properties_list:
- description: ''
  name: outputParameters
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-output-parameters2-schema.json
slug: salesforce-output-parameters2
source_filename: salesforce-output-parameters2-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"outputParameters\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"results\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"PointsDebited\": {\n                \"type\": \"integer\",\n                \"example\": 10\n              }\n            },\n            \"required\": [\n              \"PointsDebited\"\n            ]\n          }\n        }\n      },\n      \"required\": [\n        \"results\"\n      ]\n    }\n  },\n  \"required\": [\n    \"outputParameters\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OutputParameters2\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-output-parameters2-schema.json
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
title: OutputParameters2
---
