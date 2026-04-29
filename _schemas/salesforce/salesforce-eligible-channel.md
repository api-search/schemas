---
description: ''
layout: schema
name: EligibleChannel
properties_list:
- description: ''
  name: channelType
  type: string
- description: ''
  name: store
  type: object
- description: ''
  name: retailLocationGroup
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-eligible-channel-schema.json
slug: salesforce-eligible-channel
source_filename: salesforce-eligible-channel-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"channelType\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"store\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"example\": \"Example Title\"\n        }\n      },\n      \"required\": [\n        \"name\"\n      ]\n    },\n    \"retailLocationGroup\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"example\": \"Example Title\"\n        }\n      },\n      \"required\": [\n        \"name\"\n      ]\n    }\n  },\n  \"required\": [\n    \"channelType\",\n    \"store\",\n    \"retailLocationGroup\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EligibleChannel\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-eligible-channel-schema.json
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
title: EligibleChannel
---
