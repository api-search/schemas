---
description: ''
layout: schema
name: Edit
properties_list:
- description: ''
  name: isEditRestricted
  type: boolean
- description: ''
  name: isEditableByMeUrl
  type: string
- description: ''
  name: lastEditedBy
  type: '[''string'', ''null'']'
- description: ''
  name: lastEditedDate
  type: '[''string'', ''null'']'
- description: ''
  name: latestRevision
  type: integer
- description: ''
  name: relativeLastEditedDate
  type: '[''string'', ''null'']'
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-edit-schema.json
slug: salesforce-edit
source_filename: salesforce-edit-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"isEditRestricted\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"isEditableByMeUrl\": {\n      \"type\": \"string\",\n      \"example\": \"https://www.example.com\"\n    },\n    \"lastEditedBy\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"lastEditedDate\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"latestRevision\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"relativeLastEditedDate\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"isEditRestricted\",\n    \"isEditableByMeUrl\",\n    \"lastEditedBy\",\n    \"lastEditedDate\",\n    \"latestRevision\",\n    \"relativeLastEditedDate\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Edit\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-edit-schema.json
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
title: Edit
---
