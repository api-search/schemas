---
description: ''
layout: schema
name: GetCorporateHierarchyEnrichInput
properties_list:
- description: ''
  name: fieldName
  type: string
- description: ''
  name: fieldType
  type: string
- description: ''
  name: description
  type: string
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-get-corporate-hierarchy-enrich-input-schema.json
slug: zoominfo-get-corporate-hierarchy-enrich-input
source_filename: zoominfo-get-corporate-hierarchy-enrich-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"fieldName\": {\n      \"type\": \"string\",\n      \"example\": \"Acme Corporation\"\n    },\n    \"fieldType\": {\n      \"type\": \"string\",\n      \"example\": \"standard\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"example\": \"Enterprise software company\"\n    }\n  },\n  \"required\": [\n    \"fieldName\",\n    \"fieldType\",\n    \"description\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetCorporateHierarchyEnrichInput\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-get-corporate-hierarchy-enrich-input-schema.json
tags:
- B2B
- B2B Data
- Company Data
- Contact Database
- Contacts
- Data
- Lead Generation
- Marketing Intelligence
- Sales Intelligence
title: GetCorporateHierarchyEnrichInput
---
