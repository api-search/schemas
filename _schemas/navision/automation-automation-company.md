---
description: ''
layout: schema
name: AutomationCompany
properties_list:
- description: ''
  name: id
  type: string
- description: The company name
  name: name
  type: string
- description: The company display name
  name: displayName
  type: string
- description: The business profile ID
  name: businessProfileId
  type: string
- description: Whether this is an evaluation company
  name: evaluationCompany
  type: boolean
provider_name: Microsoft Dynamics NAV
provider_slug: navision
schema_file: json-schema/automation-automation-company-schema.json
slug: automation-automation-company
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AutomationCompany\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The company name\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The company display name\"\n    },\n    \"businessProfileId\": {\n      \"type\": \"string\",\n      \"description\": \"The business profile ID\"\n    },\n    \"evaluationCompany\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is an evaluation company\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/navision/refs/heads/main/json-schema/automation-automation-company-schema.json
tags:
- Business Management
- Dynamics NAV
- ERP
- Finance
- Inventory
- Microsoft
- Navision
title: AutomationCompany
---
