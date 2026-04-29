---
description: ''
layout: schema
name: Filing
properties_list:
- description: SEC filing type
  name: type
  type: string
- description: Filing date
  name: date
  type: string
- description: Filing title
  name: title
  type: string
- description: URL to SEC EDGAR filing
  name: url
  type: string
provider_name: Arch Coal
provider_slug: arch-coal
schema_file: json-schema/arch-coal-investor-relations-api-filing-schema.json
slug: arch-coal-investor-relations-api-filing
source_filename: arch-coal-investor-relations-api-filing-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"SEC filing type\",\n      \"enum\": [\n        \"10-K\",\n        \"10-Q\",\n        \"8-K\",\n        \"DEF-14A\",\n        \"SC-13G\"\n      ],\n      \"example\": \"10-K\"\n    },\n    \"date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Filing date\",\n      \"example\": \"2026-02-15\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Filing title\",\n      \"example\": \"Annual Report for Fiscal Year 2025\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"description\": \"URL to SEC EDGAR filing\",\n      \"example\": \"https://www.sec.gov/cgi-bin/browse-edgar\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/arch-coal/refs/heads/main/json-schema/arch-coal-investor-relations-api-filing-schema.json\"\
  ,\n  \"title\": \"Filing\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/arch-coal/refs/heads/main/json-schema/arch-coal-investor-relations-api-filing-schema.json
tags:
- Mining
- Coal
- Metallurgical Coal
- Thermal Coal
- Energy
- Fortune 500
title: Filing
---
