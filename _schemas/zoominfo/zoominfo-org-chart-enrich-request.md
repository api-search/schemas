---
description: ''
layout: schema
name: OrgChartEnrichRequest
properties_list:
- description: ''
  name: companyId
  type: string
- description: ''
  name: department
  type: string
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-org-chart-enrich-request-schema.json
slug: zoominfo-org-chart-enrich-request
source_filename: zoominfo-org-chart-enrich-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"companyId\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"department\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"companyId\",\n    \"department\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OrgChartEnrichRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-org-chart-enrich-request-schema.json
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
title: OrgChartEnrichRequest
---
