---
description: ''
layout: schema
name: AppUpdateRequest
properties_list:
- description: Target version to update to
  name: targetVersion
  type: string
- description: Whether to allow preview versions
  name: allowPreviewVersion
  type: boolean
- description: Whether to ignore the update window
  name: ignoreUpgradeWindow
  type: boolean
- description: Whether to also update dependent apps
  name: allowDependencyUpdate
  type: boolean
provider_name: Microsoft Dynamics NAV
provider_slug: navision
schema_file: json-schema/admin-center-app-update-request-schema.json
slug: admin-center-app-update-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AppUpdateRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"targetVersion\": {\n      \"type\": \"string\",\n      \"description\": \"Target version to update to\"\n    },\n    \"allowPreviewVersion\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to allow preview versions\"\n    },\n    \"ignoreUpgradeWindow\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to ignore the update window\"\n    },\n    \"allowDependencyUpdate\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to also update dependent apps\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/navision/refs/heads/main/json-schema/admin-center-app-update-request-schema.json
tags:
- Business Management
- Dynamics NAV
- ERP
- Finance
- Inventory
- Microsoft
- Navision
title: AppUpdateRequest
---
