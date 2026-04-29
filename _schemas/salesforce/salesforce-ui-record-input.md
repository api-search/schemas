---
description: Input for creating or updating a record
layout: schema
name: RecordInput
properties_list:
- description: The API name of the object type
  name: apiName
  type: string
- description: Field values to set, indexed by field API name
  name: fields
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-ui-record-input-schema.json
slug: salesforce-ui-record-input
source_filename: salesforce-ui-record-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Input for creating or updating a record\",\n  \"properties\": {\n    \"apiName\": {\n      \"type\": \"string\",\n      \"description\": \"The API name of the object type\",\n      \"example\": \"example_value\"\n    },\n    \"fields\": {\n      \"type\": \"object\",\n      \"description\": \"Field values to set, indexed by field API name\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"apiName\",\n    \"fields\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RecordInput\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-ui-record-input-schema.json
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
title: RecordInput
---
