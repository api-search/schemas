---
description: ''
layout: schema
name: LayoutItem
properties_list:
- description: ''
  name: editableForNew
  type: boolean
- description: ''
  name: editableForUpdate
  type: boolean
- description: ''
  name: label
  type: string
- description: ''
  name: layoutComponents
  type: array
- description: ''
  name: lookupIdApiName
  type: '[''string'', ''null'']'
- description: ''
  name: required
  type: boolean
- description: ''
  name: sortable
  type: boolean
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-layout-item-schema.json
slug: salesforce-layout-item
source_filename: salesforce-layout-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"editableForNew\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"editableForUpdate\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"label\": {\n      \"type\": \"string\",\n      \"example\": \"Example Title\"\n    },\n    \"layoutComponents\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"apiName\": {\n            \"type\": \"['string', 'null']\",\n            \"example\": \"example_value\"\n          },\n          \"componentType\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"label\": {\n            \"type\": \"string\",\n            \"example\": \"Example Title\"\n          }\n        },\n        \"required\": [\n          \"apiName\",\n          \"componentType\",\n          \"\
  label\"\n        ]\n      }\n    },\n    \"lookupIdApiName\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"required\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"sortable\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    }\n  },\n  \"required\": [\n    \"editableForNew\",\n    \"editableForUpdate\",\n    \"label\",\n    \"layoutComponents\",\n    \"lookupIdApiName\",\n    \"required\",\n    \"sortable\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LayoutItem\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-layout-item-schema.json
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
title: LayoutItem
---
