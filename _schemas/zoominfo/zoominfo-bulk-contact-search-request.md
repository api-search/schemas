---
description: ''
layout: schema
name: BulkContactSearchRequest
properties_list:
- description: ''
  name: jobType
  type: string
- description: ''
  name: query
  type: object
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-bulk-contact-search-request-schema.json
slug: zoominfo-bulk-contact-search-request
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"jobType\": {\n      \"type\": \"string\",\n      \"example\": \"standard\"\n    },\n    \"query\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"firstName\": {\n          \"type\": \"string\",\n          \"example\": \"Acme Corporation\"\n        },\n        \"companyName\": {\n          \"type\": \"string\",\n          \"example\": \"Acme Corporation\"\n        }\n      },\n      \"required\": [\n        \"firstName\",\n        \"companyName\"\n      ]\n    }\n  },\n  \"required\": [\n    \"jobType\",\n    \"query\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BulkContactSearchRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-bulk-contact-search-request-schema.json
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
title: BulkContactSearchRequest
---
