---
description: ''
layout: schema
name: UpdateSettings
properties_list:
- description: Preferred start time for the update window (UTC)
  name: preferredStartTimeUtc
  type: string
- description: Preferred end time for the update window (UTC)
  name: preferredEndTimeUtc
  type: string
provider_name: Microsoft Dynamics NAV
provider_slug: navision
schema_file: json-schema/admin-center-update-settings-schema.json
slug: admin-center-update-settings
source_filename: admin-center-update-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UpdateSettings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"preferredStartTimeUtc\": {\n      \"type\": \"string\",\n      \"description\": \"Preferred start time for the update window (UTC)\"\n    },\n    \"preferredEndTimeUtc\": {\n      \"type\": \"string\",\n      \"description\": \"Preferred end time for the update window (UTC)\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/navision/refs/heads/main/json-schema/admin-center-update-settings-schema.json
tags:
- Business Management
- Dynamics NAV
- ERP
- Finance
- Inventory
- Microsoft
- Navision
title: UpdateSettings
---
