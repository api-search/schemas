---
description: ''
layout: schema
name: result3
properties_list:
- description: ''
  name: metadataObjects
  type: array
- description: ''
  name: organizationNamespace
  type: string
- description: ''
  name: partialSaveAllowed
  type: boolean
- description: ''
  name: testRequired
  type: boolean
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-result3-schema.json
slug: salesforce-result3
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"metadataObjects\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"directoryName\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"inFolder\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"metaFile\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"suffix\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"xmlName\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"childXmlNames\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          }\n        },\n        \"required\": [\n          \"\
  directoryName\",\n          \"inFolder\",\n          \"metaFile\",\n          \"xmlName\"\n        ]\n      }\n    },\n    \"organizationNamespace\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"partialSaveAllowed\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"testRequired\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    }\n  },\n  \"required\": [\n    \"metadataObjects\",\n    \"organizationNamespace\",\n    \"partialSaveAllowed\",\n    \"testRequired\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"result3\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-result3-schema.json
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
title: result3
---
