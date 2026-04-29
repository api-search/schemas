---
description: ''
layout: schema
name: CreateaRecordRequest
properties_list:
- description: ''
  name: allowSaveOnDuplicate
  type: boolean
- description: ''
  name: apiName
  type: string
- description: ''
  name: fields
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-createa-record-request-schema.json
slug: salesforce-createa-record-request
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"allowSaveOnDuplicate\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"apiName\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"fields\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"FieldAPIName\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"FieldAPIName\"\n      ]\n    }\n  },\n  \"required\": [\n    \"allowSaveOnDuplicate\",\n    \"apiName\",\n    \"fields\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateaRecordRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-createa-record-request-schema.json
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
title: CreateaRecordRequest
---
