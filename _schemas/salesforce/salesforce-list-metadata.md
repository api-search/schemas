---
description: ''
layout: schema
name: listMetadata
properties_list:
- description: ''
  name: listMetadataQuery
  type: object
- description: ''
  name: asOfVersion
  type: number
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-list-metadata-schema.json
slug: salesforce-list-metadata
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"listMetadataQuery\": {\n      \"type\": \"object\",\n      \"example\": \"example_value\"\n    },\n    \"asOfVersion\": {\n      \"type\": \"number\",\n      \"example\": 42.5\n    }\n  },\n  \"required\": [\n    \"listMetadataQuery\",\n    \"asOfVersion\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"listMetadata\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-list-metadata-schema.json
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
title: listMetadata
---
