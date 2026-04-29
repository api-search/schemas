---
description: ''
layout: schema
name: metadataObjects
properties_list:
- description: ''
  name: directoryName
  type: string
- description: ''
  name: inFolder
  type: boolean
- description: ''
  name: metaFile
  type: boolean
- description: ''
  name: suffix
  type: string
- description: ''
  name: xmlName
  type: string
- description: ''
  name: childXmlNames
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-metadata-objects-schema.json
slug: salesforce-metadata-objects
source_filename: salesforce-metadata-objects-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"directoryName\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"inFolder\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"metaFile\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"suffix\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"xmlName\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"childXmlNames\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"directoryName\",\n    \"inFolder\",\n    \"metaFile\",\n    \"xmlName\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"metadataObjects\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-metadata-objects-schema.json
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
title: metadataObjects
---
