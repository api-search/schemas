---
description: ''
layout: schema
name: RecordTypeInfo
properties_list:
- description: ''
  name: active
  type: boolean
- description: ''
  name: available
  type: boolean
- description: ''
  name: defaultRecordTypeMapping
  type: boolean
- description: ''
  name: developerName
  type: string
- description: ''
  name: master
  type: boolean
- description: ''
  name: name
  type: string
- description: ''
  name: recordTypeId
  type: string
- description: ''
  name: urls
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-record-type-info-schema.json
slug: salesforce-record-type-info
source_filename: salesforce-record-type-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"active\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"available\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"defaultRecordTypeMapping\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"developerName\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"master\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"Example Title\"\n    },\n    \"recordTypeId\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"urls\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"layout\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"layout\"\n      ]\n    }\n  },\n  \"required\": [\n    \"active\",\n    \"available\"\
  ,\n    \"defaultRecordTypeMapping\",\n    \"developerName\",\n    \"master\",\n    \"name\",\n    \"recordTypeId\",\n    \"urls\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RecordTypeInfo\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-record-type-info-schema.json
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
title: RecordTypeInfo
---
