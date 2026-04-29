---
description: ''
layout: schema
name: ScheduledUpgrade
properties_list:
- description: ''
  name: environmentName
  type: string
- description: ''
  name: upgradeIsScheduled
  type: boolean
- description: ''
  name: scheduledDate
  type: string
- description: ''
  name: registeredDate
  type: string
- description: ''
  name: targetVersion
  type: string
- description: ''
  name: canTenantSelectDate
  type: boolean
- description: ''
  name: ignoreUpgradeWindow
  type: boolean
provider_name: Microsoft Dynamics NAV
provider_slug: navision
schema_file: json-schema/admin-center-scheduled-upgrade-schema.json
slug: admin-center-scheduled-upgrade
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ScheduledUpgrade\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"environmentName\": {\n      \"type\": \"string\"\n    },\n    \"upgradeIsScheduled\": {\n      \"type\": \"boolean\"\n    },\n    \"scheduledDate\": {\n      \"type\": \"string\"\n    },\n    \"registeredDate\": {\n      \"type\": \"string\"\n    },\n    \"targetVersion\": {\n      \"type\": \"string\"\n    },\n    \"canTenantSelectDate\": {\n      \"type\": \"boolean\"\n    },\n    \"ignoreUpgradeWindow\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/navision/refs/heads/main/json-schema/admin-center-scheduled-upgrade-schema.json
tags:
- Business Management
- Dynamics NAV
- ERP
- Finance
- Inventory
- Microsoft
- Navision
title: ScheduledUpgrade
---
