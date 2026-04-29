---
description: ''
layout: schema
name: Record9
properties_list:
- description: ''
  name: attributes
  type: object
- description: ''
  name: Id
  type: string
- description: ''
  name: DeveloperName
  type: string
- description: ''
  name: MasterLabel
  type: string
- description: ''
  name: ChannelType
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-record9-schema.json
slug: salesforce-record9
source_filename: salesforce-record9-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"attributes\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"url\": {\n          \"type\": \"string\",\n          \"example\": \"https://www.example.com\"\n        }\n      },\n      \"required\": [\n        \"type\",\n        \"url\"\n      ]\n    },\n    \"Id\": {\n      \"type\": \"string\",\n      \"example\": \"abc123\"\n    },\n    \"DeveloperName\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"MasterLabel\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"ChannelType\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"attributes\",\n    \"Id\",\n    \"DeveloperName\",\n    \"MasterLabel\",\n    \"ChannelType\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\"\
  ,\n  \"title\": \"Record9\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-record9-schema.json
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
title: Record9
---
