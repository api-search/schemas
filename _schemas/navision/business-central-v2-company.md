---
description: ''
layout: schema
name: Company
properties_list:
- description: The unique identifier of the company
  name: id
  type: string
- description: The system version
  name: systemVersion
  type: string
- description: The name of the company
  name: name
  type: string
- description: The display name of the company
  name: displayName
  type: string
- description: The business profile ID
  name: businessProfileId
  type: string
provider_name: Microsoft Dynamics NAV
provider_slug: navision
schema_file: json-schema/business-central-v2-company-schema.json
slug: business-central-v2-company
source_filename: business-central-v2-company-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Company\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the company\"\n    },\n    \"systemVersion\": {\n      \"type\": \"string\",\n      \"description\": \"The system version\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the company\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the company\"\n    },\n    \"businessProfileId\": {\n      \"type\": \"string\",\n      \"description\": \"The business profile ID\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/navision/refs/heads/main/json-schema/business-central-v2-company-schema.json
tags:
- Business Management
- Dynamics NAV
- ERP
- Finance
- Inventory
- Microsoft
- Navision
title: Company
---
