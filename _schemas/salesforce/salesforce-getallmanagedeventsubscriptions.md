---
description: ''
layout: schema
name: Getallmanagedeventsubscriptions
properties_list:
- description: ''
  name: size
  type: integer
- description: ''
  name: totalSize
  type: integer
- description: ''
  name: done
  type: boolean
- description: ''
  name: queryLocator
  type: '[''string'', ''null'']'
- description: ''
  name: entityTypeName
  type: string
- description: ''
  name: records
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-getallmanagedeventsubscriptions-schema.json
slug: salesforce-getallmanagedeventsubscriptions
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"size\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"totalSize\": {\n      \"type\": \"integer\",\n      \"example\": 42\n    },\n    \"done\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"queryLocator\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"entityTypeName\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"records\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"attributes\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"type\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              },\n              \"url\": {\n                \"type\": \"string\",\n           \
  \     \"example\": \"https://www.example.com\"\n              }\n            },\n            \"required\": [\n              \"type\",\n              \"url\"\n            ]\n          },\n          \"Id\": {\n            \"type\": \"string\",\n            \"example\": \"abc123\"\n          },\n          \"IsDeleted\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"DeveloperName\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"Language\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"MasterLabel\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"NamespacePrefix\": {\n            \"type\": \"['string', 'null']\",\n            \"example\": \"example_value\"\n          },\n          \"ManageableState\": {\n            \"type\": \"string\",\n            \"example\"\
  : \"example_value\"\n          },\n          \"CreatedDate\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"CreatedById\": {\n            \"type\": \"string\",\n            \"example\": \"500123\"\n          },\n          \"LastModifiedDate\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"LastModifiedById\": {\n            \"type\": \"string\",\n            \"example\": \"500123\"\n          },\n          \"SystemModstamp\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"Version\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          }\n        },\n        \"required\": [\n          \"attributes\",\n          \"Id\",\n          \"IsDeleted\",\n          \"DeveloperName\",\n          \"Language\",\n          \"MasterLabel\",\n          \"NamespacePrefix\",\n        \
  \  \"ManageableState\",\n          \"CreatedDate\",\n          \"CreatedById\",\n          \"LastModifiedDate\",\n          \"LastModifiedById\",\n          \"SystemModstamp\",\n          \"Version\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"size\",\n    \"totalSize\",\n    \"done\",\n    \"queryLocator\",\n    \"entityTypeName\",\n    \"records\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Getallmanagedeventsubscriptions\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-getallmanagedeventsubscriptions-schema.json
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
title: Getallmanagedeventsubscriptions
---
