---
description: ''
layout: schema
name: Subject
properties_list:
- description: ''
  name: entityLabel
  type: object
- description: ''
  name: id
  type: string
- description: ''
  name: motif
  type: object
- description: ''
  name: mySubscription
  type: '[''string'', ''null'']'
- description: ''
  name: name
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: url
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-subject-schema.json
slug: salesforce-subject
source_filename: salesforce-subject-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"entityLabel\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"label\": {\n          \"type\": \"string\",\n          \"example\": \"Example Title\"\n        },\n        \"labelPlural\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"label\",\n        \"labelPlural\"\n      ]\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"example\": \"abc123\"\n    },\n    \"motif\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"color\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"largeIconUrl\": {\n          \"type\": \"string\",\n          \"example\": \"https://www.example.com\"\n        },\n        \"mediumIconUrl\": {\n          \"type\": \"string\",\n          \"example\": \"https://www.example.com\"\n        },\n        \"smallIconUrl\":\
  \ {\n          \"type\": \"string\",\n          \"example\": \"https://www.example.com\"\n        },\n        \"svgIconUrl\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"https://www.example.com\"\n        }\n      },\n      \"required\": [\n        \"color\",\n        \"largeIconUrl\",\n        \"mediumIconUrl\",\n        \"smallIconUrl\",\n        \"svgIconUrl\"\n      ]\n    },\n    \"mySubscription\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"Example Title\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"example\": \"https://www.example.com\"\n    }\n  },\n  \"required\": [\n    \"entityLabel\",\n    \"id\",\n    \"motif\",\n    \"mySubscription\",\n    \"name\",\n    \"type\",\n    \"url\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\"\
  ,\n  \"title\": \"Subject\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-subject-schema.json
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
title: Subject
---
