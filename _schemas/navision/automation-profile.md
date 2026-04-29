---
description: ''
layout: schema
name: Profile
properties_list:
- description: The profile ID
  name: profileId
  type: string
- description: ''
  name: scope
  type: string
- description: The profile caption
  name: caption
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: applicationId
  type: string
- description: ''
  name: enabled
  type: boolean
provider_name: Microsoft Dynamics NAV
provider_slug: navision
schema_file: json-schema/automation-profile-schema.json
slug: automation-profile
source_filename: automation-profile-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Profile\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"profileId\": {\n      \"type\": \"string\",\n      \"description\": \"The profile ID\"\n    },\n    \"scope\": {\n      \"type\": \"string\"\n    },\n    \"caption\": {\n      \"type\": \"string\",\n      \"description\": \"The profile caption\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"applicationId\": {\n      \"type\": \"string\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/navision/refs/heads/main/json-schema/automation-profile-schema.json
tags:
- Business Management
- Dynamics NAV
- ERP
- Finance
- Inventory
- Microsoft
- Navision
title: Profile
---
