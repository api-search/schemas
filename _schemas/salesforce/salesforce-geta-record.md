---
description: ''
layout: schema
name: GetaRecord
properties_list:
- description: ''
  name: apiName
  type: string
- description: ''
  name: childRelationships
  type: object
- description: ''
  name: eTag
  type: string
- description: ''
  name: fields
  type: object
- description: ''
  name: id
  type: string
- description: ''
  name: lastModifiedById
  type: string
- description: ''
  name: lastModifiedDate
  type: string
- description: ''
  name: recordTypeId
  type: string
- description: ''
  name: recordTypeInfo
  type: '[''string'', ''null'']'
- description: ''
  name: systemModstamp
  type: string
- description: ''
  name: weakEtag
  type: integer
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-geta-record-schema.json
slug: salesforce-geta-record
source_filename: salesforce-geta-record-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"apiName\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"childRelationships\": {\n      \"type\": \"object\",\n      \"example\": \"example_value\"\n    },\n    \"eTag\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"fields\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Name\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"displayValue\": {\n              \"type\": \"['string', 'null']\",\n              \"example\": \"example_value\"\n            },\n            \"value\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            }\n          },\n          \"required\": [\n            \"displayValue\",\n            \"value\"\n          ]\n        },\n        \"Rating\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"displayValue\"\
  : {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            },\n            \"value\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            }\n          },\n          \"required\": [\n            \"displayValue\",\n            \"value\"\n          ]\n        }\n      },\n      \"required\": [\n        \"Name\",\n        \"Rating\"\n      ]\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"example\": \"abc123\"\n    },\n    \"lastModifiedById\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"lastModifiedDate\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"recordTypeId\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"recordTypeInfo\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"systemModstamp\": {\n      \"type\": \"string\",\n      \"example\"\
  : \"example_value\"\n    },\n    \"weakEtag\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    }\n  },\n  \"required\": [\n    \"apiName\",\n    \"childRelationships\",\n    \"eTag\",\n    \"fields\",\n    \"id\",\n    \"lastModifiedById\",\n    \"lastModifiedDate\",\n    \"recordTypeId\",\n    \"recordTypeInfo\",\n    \"systemModstamp\",\n    \"weakEtag\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetaRecord\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-geta-record-schema.json
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
title: GetaRecord
---
