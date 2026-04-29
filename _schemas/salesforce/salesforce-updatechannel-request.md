---
description: ''
layout: schema
name: UpdatechannelRequest
properties_list:
- description: ''
  name: FullName
  type: string
- description: ''
  name: Metadata
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-updatechannel-request-schema.json
slug: salesforce-updatechannel-request
source_filename: salesforce-updatechannel-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"FullName\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"Metadata\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"channelType\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"label\": {\n          \"type\": \"string\",\n          \"example\": \"Example Title\"\n        },\n        \"urls\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"https://www.example.com\"\n        }\n      },\n      \"required\": [\n        \"channelType\",\n        \"label\",\n        \"urls\"\n      ]\n    }\n  },\n  \"required\": [\n    \"FullName\",\n    \"Metadata\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UpdatechannelRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-updatechannel-request-schema.json
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
title: UpdatechannelRequest
---
