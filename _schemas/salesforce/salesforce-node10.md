---
description: ''
layout: schema
name: Node10
properties_list:
- description: ''
  name: Id
  type: string
- description: ''
  name: Name
  type: object
- description: ''
  name: CloseDate
  type: object
- description: ''
  name: StageName
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-node10-schema.json
slug: salesforce-node10
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"example\": \"abc123\"\n    },\n    \"Name\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"value\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"value\"\n      ]\n    },\n    \"CloseDate\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"value\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"displayValue\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"value\",\n        \"displayValue\"\n      ]\n    },\n    \"StageName\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"value\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\"\
  : [\n        \"value\"\n      ]\n    }\n  },\n  \"required\": [\n    \"Id\",\n    \"Name\",\n    \"CloseDate\",\n    \"StageName\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Node10\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-node10-schema.json
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
title: Node10
---
