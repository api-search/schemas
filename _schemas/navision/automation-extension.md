---
description: ''
layout: schema
name: Extension
properties_list:
- description: The extension ID
  name: id
  type: string
- description: The package ID used for install/uninstall operations
  name: packageId
  type: string
- description: The extension display name
  name: displayName
  type: string
- description: The extension publisher
  name: publisher
  type: string
- description: Major version number
  name: versionMajor
  type: integer
- description: Minor version number
  name: versionMinor
  type: integer
- description: Build version number
  name: versionBuild
  type: integer
- description: Revision version number
  name: versionRevision
  type: integer
- description: Whether the extension is currently installed
  name: isInstalled
  type: boolean
- description: How the extension was published
  name: publishedAs
  type: string
provider_name: Microsoft Dynamics NAV
provider_slug: navision
schema_file: json-schema/automation-extension-schema.json
slug: automation-extension
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Extension\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The extension ID\"\n    },\n    \"packageId\": {\n      \"type\": \"string\",\n      \"description\": \"The package ID used for install/uninstall operations\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The extension display name\"\n    },\n    \"publisher\": {\n      \"type\": \"string\",\n      \"description\": \"The extension publisher\"\n    },\n    \"versionMajor\": {\n      \"type\": \"integer\",\n      \"description\": \"Major version number\"\n    },\n    \"versionMinor\": {\n      \"type\": \"integer\",\n      \"description\": \"Minor version number\"\n    },\n    \"versionBuild\": {\n      \"type\": \"integer\",\n      \"description\": \"Build version number\"\n    },\n    \"versionRevision\": {\n      \"type\":\
  \ \"integer\",\n      \"description\": \"Revision version number\"\n    },\n    \"isInstalled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the extension is currently installed\"\n    },\n    \"publishedAs\": {\n      \"type\": \"string\",\n      \"description\": \"How the extension was published\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/navision/refs/heads/main/json-schema/automation-extension-schema.json
tags:
- Business Management
- Dynamics NAV
- ERP
- Finance
- Inventory
- Microsoft
- Navision
title: Extension
---
