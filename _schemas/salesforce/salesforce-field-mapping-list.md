---
description: ''
layout: schema
name: FieldMappingList
properties_list:
- description: ''
  name: modelField
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-field-mapping-list-schema.json
slug: salesforce-field-mapping-list
source_filename: salesforce-field-mapping-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"modelField\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"label\": {\n          \"type\": \"string\",\n          \"example\": \"Example Title\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"example\": \"Example Title\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"label\",\n        \"name\",\n        \"type\"\n      ]\n    }\n  },\n  \"required\": [\n    \"modelField\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"FieldMappingList\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-field-mapping-list-schema.json
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
title: FieldMappingList
---
