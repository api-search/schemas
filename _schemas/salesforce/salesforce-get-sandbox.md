---
description: ''
layout: schema
name: GetSandbox
properties_list:
- description: ''
  name: attributes
  type: object
- description: ''
  name: Id
  type: string
- description: ''
  name: IsDeleted
  type: boolean
- description: ''
  name: CreatedDate
  type: string
- description: ''
  name: CreatedById
  type: string
- description: ''
  name: LastModifiedDate
  type: string
- description: ''
  name: LastModifiedById
  type: string
- description: ''
  name: SystemModstamp
  type: string
- description: ''
  name: SandboxName
  type: string
- description: ''
  name: LicenseType
  type: string
- description: ''
  name: TemplateId
  type: '[''string'', ''null'']'
- description: ''
  name: HistoryDays
  type: integer
- description: ''
  name: CopyChatter
  type: boolean
- description: ''
  name: AutoActivate
  type: boolean
- description: ''
  name: ApexClassId
  type: '[''string'', ''null'']'
- description: ''
  name: Description
  type: string
- description: ''
  name: SourceId
  type: '[''string'', ''null'']'
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-get-sandbox-schema.json
slug: salesforce-get-sandbox
source_filename: salesforce-get-sandbox-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"attributes\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"url\": {\n          \"type\": \"string\",\n          \"example\": \"https://www.example.com\"\n        }\n      },\n      \"required\": [\n        \"type\",\n        \"url\"\n      ]\n    },\n    \"Id\": {\n      \"type\": \"string\",\n      \"example\": \"abc123\"\n    },\n    \"IsDeleted\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"CreatedDate\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"CreatedById\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"LastModifiedDate\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"LastModifiedById\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n\
  \    },\n    \"SystemModstamp\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"SandboxName\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"LicenseType\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"TemplateId\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"500123\"\n    },\n    \"HistoryDays\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"CopyChatter\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"AutoActivate\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"ApexClassId\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"500123\"\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"example\": \"A sample description.\"\n    },\n    \"SourceId\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"500123\"\n    }\n  },\n  \"required\"\
  : [\n    \"attributes\",\n    \"Id\",\n    \"IsDeleted\",\n    \"CreatedDate\",\n    \"CreatedById\",\n    \"LastModifiedDate\",\n    \"LastModifiedById\",\n    \"SystemModstamp\",\n    \"SandboxName\",\n    \"LicenseType\",\n    \"TemplateId\",\n    \"HistoryDays\",\n    \"CopyChatter\",\n    \"AutoActivate\",\n    \"ApexClassId\",\n    \"Description\",\n    \"SourceId\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetSandbox\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-get-sandbox-schema.json
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
title: GetSandbox
---
