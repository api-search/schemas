---
description: ''
layout: schema
name: AddenrichedfieldstochannelmemberRequest
properties_list:
- description: ''
  name: FullName
  type: string
- description: ''
  name: Metadata
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-addenrichedfieldstochannelmember-request-schema.json
slug: salesforce-addenrichedfieldstochannelmember-request
source_filename: salesforce-addenrichedfieldstochannelmember-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"FullName\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"Metadata\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"enrichedFields\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"name\": {\n                \"type\": \"string\",\n                \"example\": \"Example Title\"\n              }\n            },\n            \"required\": [\n              \"name\"\n            ]\n          }\n        },\n        \"eventChannel\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"selectedEntity\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"enrichedFields\",\n        \"eventChannel\"\
  ,\n        \"selectedEntity\"\n      ]\n    }\n  },\n  \"required\": [\n    \"FullName\",\n    \"Metadata\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AddenrichedfieldstochannelmemberRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-addenrichedfieldstochannelmember-request-schema.json
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
title: AddenrichedfieldstochannelmemberRequest
---
