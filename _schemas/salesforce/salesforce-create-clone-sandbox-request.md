---
description: ''
layout: schema
name: CreateCloneSandboxRequest
properties_list:
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
schema_file: json-schema/salesforce-create-clone-sandbox-request-schema.json
slug: salesforce-create-clone-sandbox-request
source_filename: salesforce-create-clone-sandbox-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"SandboxName\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"LicenseType\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"TemplateId\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"500123\"\n    },\n    \"HistoryDays\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"CopyChatter\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"AutoActivate\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"ApexClassId\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"500123\"\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"example\": \"A sample description.\"\n    },\n    \"SourceId\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"500123\"\n    }\n  },\n  \"required\": [\n    \"SandboxName\",\n    \"LicenseType\"\
  ,\n    \"TemplateId\",\n    \"HistoryDays\",\n    \"CopyChatter\",\n    \"AutoActivate\",\n    \"ApexClassId\",\n    \"Description\",\n    \"SourceId\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateCloneSandboxRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-create-clone-sandbox-request-schema.json
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
title: CreateCloneSandboxRequest
---
