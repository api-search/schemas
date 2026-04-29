---
description: A single picklist option
layout: schema
name: PicklistValue
properties_list:
- description: ''
  name: attributes
  type: object
- description: ''
  name: label
  type: string
- description: ''
  name: validFor
  type: array
- description: ''
  name: value
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-ui-picklist-value-schema.json
slug: salesforce-ui-picklist-value
source_filename: salesforce-ui-picklist-value-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A single picklist option\",\n  \"properties\": {\n    \"attributes\": {\n      \"type\": \"object\",\n      \"example\": \"example_value\"\n    },\n    \"label\": {\n      \"type\": \"string\",\n      \"example\": \"Example Title\"\n    },\n    \"validFor\": {\n      \"type\": \"array\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"integer\"\n      }\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PicklistValue\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-ui-picklist-value-schema.json
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
title: PicklistValue
---
