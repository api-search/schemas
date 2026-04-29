---
description: ''
layout: schema
name: ChildRelationship
properties_list:
- description: ''
  name: cascadeDelete
  type: boolean
- description: ''
  name: childSObject
  type: string
- description: ''
  name: deprecatedAndHidden
  type: boolean
- description: ''
  name: field
  type: string
- description: ''
  name: junctionIdListNames
  type: array
- description: ''
  name: junctionReferenceTo
  type: array
- description: ''
  name: relationshipName
  type: '[''string'', ''null'']'
- description: ''
  name: restrictedDelete
  type: boolean
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-child-relationship-schema.json
slug: salesforce-child-relationship
source_filename: salesforce-child-relationship-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"cascadeDelete\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"childSObject\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"deprecatedAndHidden\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"field\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"junctionIdListNames\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"junctionReferenceTo\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"relationshipName\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"restrictedDelete\": {\n      \"type\": \"boolean\",\n      \"example\": true\n\
  \    }\n  },\n  \"required\": [\n    \"cascadeDelete\",\n    \"childSObject\",\n    \"deprecatedAndHidden\",\n    \"field\",\n    \"junctionIdListNames\",\n    \"junctionReferenceTo\",\n    \"relationshipName\",\n    \"restrictedDelete\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ChildRelationship\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-child-relationship-schema.json
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
title: ChildRelationship
---
