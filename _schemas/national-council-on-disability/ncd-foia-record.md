---
description: A record available through the National Council on Disability's FOIA e-Library.
layout: schema
name: NCD FOIA Record
properties_list:
- description: Type of FOIA record
  name: recordType
  type: string
- description: Document title
  name: title
  type: string
- description: Fiscal year of the record (e.g., FY2025)
  name: fiscalYear
  type: string
- description: Date published to FOIA library
  name: publishedDate
  type: string
- description: URL to access the document
  name: documentURL
  type: string
- description: Document format
  name: format
  type: string
- description: Brief description of the record contents
  name: description
  type: string
provider_name: National Council on Disability
provider_slug: national-council-on-disability
schema_file: json-schema/ncd-foia-record-schema.json
slug: ncd-foia-record
source_filename: ncd-foia-record-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://www.ncd.gov/schemas/foia-record\",\n  \"title\": \"NCD FOIA Record\",\n  \"description\": \"A record available through the National Council on Disability's FOIA e-Library.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"recordType\",\n    \"title\",\n    \"fiscalYear\"\n  ],\n  \"properties\": {\n    \"recordType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Bylaws\",\n        \"PerformanceReport\",\n        \"BudgetJustification\",\n        \"FinancialAudit\",\n        \"StrategicPlan\",\n        \"StakeholderLetter\",\n        \"PolicyReport\",\n        \"FOIAReport\"\n      ],\n      \"description\": \"Type of FOIA record\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Document title\"\n    },\n    \"fiscalYear\": {\n      \"type\": \"string\",\n      \"description\": \"Fiscal year of the record (e.g., FY2025)\"\n    },\n  \
  \  \"publishedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date published to FOIA library\"\n    },\n    \"documentURL\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to access the document\"\n    },\n    \"format\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"PDF\",\n        \"XML\",\n        \"CSV\",\n        \"ZIP\"\n      ],\n      \"description\": \"Document format\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Brief description of the record contents\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/national-council-on-disability/refs/heads/main/json-schema/ncd-foia-record-schema.json
tags:
- Disability
- Federal Government
- Policy
- Civil Rights
- Healthcare
- Independent Agency
title: NCD FOIA Record
---
