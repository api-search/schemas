---
description: ''
layout: schema
name: RestoreEnvironmentRequest
properties_list:
- description: Name of the new restored environment
  name: EnvironmentName
  type: string
- description: Type of the new environment
  name: EnvironmentType
  type: string
- description: Point in time to restore to (ISO 8601 UTC)
  name: PointInTime
  type: string
- description: Whether to uninstall per-tenant extensions
  name: SkipInstallingPTEs
  type: boolean
- description: Whether to uninstall third-party AppSource apps
  name: SkipInstallingThirdPartyGlobalApps
  type: boolean
- description: Whether to skip execution of cleanup codeunits
  name: SkipEnvironmentCleanup
  type: boolean
provider_name: Microsoft Dynamics NAV
provider_slug: navision
schema_file: json-schema/admin-center-restore-environment-request-schema.json
slug: admin-center-restore-environment-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RestoreEnvironmentRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EnvironmentName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the new restored environment\"\n    },\n    \"EnvironmentType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of the new environment\"\n    },\n    \"PointInTime\": {\n      \"type\": \"string\",\n      \"description\": \"Point in time to restore to (ISO 8601 UTC)\"\n    },\n    \"SkipInstallingPTEs\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to uninstall per-tenant extensions\"\n    },\n    \"SkipInstallingThirdPartyGlobalApps\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to uninstall third-party AppSource apps\"\n    },\n    \"SkipEnvironmentCleanup\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to skip execution of cleanup codeunits\"\n   \
  \ }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/navision/refs/heads/main/json-schema/admin-center-restore-environment-request-schema.json
tags:
- Business Management
- Dynamics NAV
- ERP
- Finance
- Inventory
- Microsoft
- Navision
title: RestoreEnvironmentRequest
---
