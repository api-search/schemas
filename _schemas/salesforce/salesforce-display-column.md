---
description: ''
layout: schema
name: DisplayColumn
properties_list:
- description: ''
  name: fieldApiName
  type: string
- description: ''
  name: inlineEditAttributes
  type: object
- description: ''
  name: label
  type: string
- description: ''
  name: lookupId
  type: '[''string'', ''null'']'
- description: ''
  name: searchable
  type: boolean
- description: ''
  name: sortable
  type: boolean
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-display-column-schema.json
slug: salesforce-display-column
source_filename: salesforce-display-column-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"fieldApiName\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"inlineEditAttributes\": {\n      \"type\": \"object\",\n      \"example\": \"example_value\"\n    },\n    \"label\": {\n      \"type\": \"string\",\n      \"example\": \"Example Title\"\n    },\n    \"lookupId\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"500123\"\n    },\n    \"searchable\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"sortable\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    }\n  },\n  \"required\": [\n    \"fieldApiName\",\n    \"inlineEditAttributes\",\n    \"label\",\n    \"lookupId\",\n    \"searchable\",\n    \"sortable\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DisplayColumn\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-display-column-schema.json
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
title: DisplayColumn
---
