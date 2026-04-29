---
description: ''
layout: schema
name: PageReference
properties_list:
- description: ''
  name: attributes
  type: object
- description: ''
  name: state
  type: object
- description: ''
  name: type
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-page-reference-schema.json
slug: salesforce-page-reference
source_filename: salesforce-page-reference-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"attributes\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"pageName\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"objectApiName\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"actionName\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      }\n    },\n    \"state\": {\n      \"type\": \"object\",\n      \"example\": \"example_value\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"attributes\",\n    \"state\",\n    \"type\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PageReference\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-page-reference-schema.json
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
title: PageReference
---
