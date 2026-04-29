---
description: ''
layout: schema
name: ScorecardAssociation
properties_list:
- description: ''
  name: apiName
  type: string
- description: ''
  name: keyPrefix
  type: string
- description: ''
  name: label
  type: string
- description: ''
  name: labelPlural
  type: string
- description: ''
  name: nameFields
  type: array
- description: ''
  name: objectInfoUrl
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-scorecard-association-schema.json
slug: salesforce-scorecard-association
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"apiName\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"keyPrefix\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"label\": {\n      \"type\": \"string\",\n      \"example\": \"Example Title\"\n    },\n    \"labelPlural\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"nameFields\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"objectInfoUrl\": {\n      \"type\": \"string\",\n      \"example\": \"https://www.example.com\"\n    }\n  },\n  \"required\": [\n    \"apiName\",\n    \"keyPrefix\",\n    \"label\",\n    \"labelPlural\",\n    \"nameFields\",\n    \"objectInfoUrl\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ScorecardAssociation\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-scorecard-association-schema.json
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
title: ScorecardAssociation
---
