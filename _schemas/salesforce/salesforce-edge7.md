---
description: ''
layout: schema
name: Edge7
properties_list:
- description: ''
  name: node
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-edge7-schema.json
slug: salesforce-edge7
source_filename: salesforce-edge7-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"node\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Id\": {\n          \"type\": \"string\",\n          \"example\": \"abc123\"\n        },\n        \"Name\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"value\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            }\n          },\n          \"required\": [\n            \"value\"\n          ]\n        },\n        \"StageName\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"value\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            }\n          },\n          \"required\": [\n            \"value\"\n          ]\n        },\n        \"CloseDate\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"value\": {\n              \"type\": \"string\",\n              \"example\"\
  : \"example_value\"\n            },\n            \"displayValue\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            }\n          },\n          \"required\": [\n            \"value\",\n            \"displayValue\"\n          ]\n        },\n        \"Description\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"value\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            }\n          },\n          \"required\": [\n            \"value\"\n          ]\n        }\n      },\n      \"required\": [\n        \"Id\",\n        \"Name\",\n        \"StageName\",\n        \"CloseDate\",\n        \"Description\"\n      ]\n    }\n  },\n  \"required\": [\n    \"node\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Edge7\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-edge7-schema.json
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
title: Edge7
---
