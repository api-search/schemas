---
description: ''
layout: schema
name: CompanyMasterDataEnrichOutput
properties_list:
- description: ''
  name: fieldName
  type: string
- description: ''
  name: dataType
  type: string
- description: ''
  name: description
  type: string
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-company-master-data-enrich-output-schema.json
slug: zoominfo-company-master-data-enrich-output
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"fieldName\": {\n      \"type\": \"string\",\n      \"example\": \"Acme Corporation\"\n    },\n    \"dataType\": {\n      \"type\": \"string\",\n      \"example\": \"standard\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"example\": \"Enterprise software company\"\n    }\n  },\n  \"required\": [\n    \"fieldName\",\n    \"dataType\",\n    \"description\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CompanyMasterDataEnrichOutput\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-company-master-data-enrich-output-schema.json
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
title: CompanyMasterDataEnrichOutput
---
