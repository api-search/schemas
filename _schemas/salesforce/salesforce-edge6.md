---
description: ''
layout: schema
name: Edge6
properties_list:
- description: ''
  name: node
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-edge6-schema.json
slug: salesforce-edge6
source_filename: salesforce-edge6-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"node\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Id\": {\n          \"type\": \"string\",\n          \"example\": \"abc123\"\n        },\n        \"Name\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"value\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            }\n          },\n          \"required\": [\n            \"value\"\n          ]\n        },\n        \"Account\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"Name\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"value\": {\n                  \"type\": \"string\",\n                  \"example\": \"example_value\"\n                }\n              },\n              \"required\": [\n                \"value\"\n              ]\n            }\n          },\n          \"required\": [\n  \
  \          \"Name\"\n          ]\n        }\n      },\n      \"required\": [\n        \"Id\",\n        \"Name\",\n        \"Account\"\n      ]\n    }\n  },\n  \"required\": [\n    \"node\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Edge6\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-edge6-schema.json
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
title: Edge6
---
