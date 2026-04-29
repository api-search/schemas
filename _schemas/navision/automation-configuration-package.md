---
description: ''
layout: schema
name: ConfigurationPackage
properties_list:
- description: ''
  name: id
  type: string
- description: The package code
  name: code
  type: string
- description: The package name
  name: packageName
  type: string
- description: ''
  name: languageId
  type: integer
- description: ''
  name: productVersion
  type: string
- description: ''
  name: processingOrder
  type: integer
- description: ''
  name: excludeConfigurationTables
  type: boolean
- description: ''
  name: numberOfTables
  type: integer
- description: ''
  name: numberOfRecords
  type: integer
- description: ''
  name: numberOfErrors
  type: integer
- description: ''
  name: importStatus
  type: string
- description: ''
  name: applyStatus
  type: string
provider_name: Microsoft Dynamics NAV
provider_slug: navision
schema_file: json-schema/automation-configuration-package-schema.json
slug: automation-configuration-package
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ConfigurationPackage\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"The package code\"\n    },\n    \"packageName\": {\n      \"type\": \"string\",\n      \"description\": \"The package name\"\n    },\n    \"languageId\": {\n      \"type\": \"integer\"\n    },\n    \"productVersion\": {\n      \"type\": \"string\"\n    },\n    \"processingOrder\": {\n      \"type\": \"integer\"\n    },\n    \"excludeConfigurationTables\": {\n      \"type\": \"boolean\"\n    },\n    \"numberOfTables\": {\n      \"type\": \"integer\"\n    },\n    \"numberOfRecords\": {\n      \"type\": \"integer\"\n    },\n    \"numberOfErrors\": {\n      \"type\": \"integer\"\n    },\n    \"importStatus\": {\n      \"type\": \"string\"\n    },\n    \"applyStatus\": {\n      \"type\": \"string\"\n    }\n\
  \  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/navision/refs/heads/main/json-schema/automation-configuration-package-schema.json
tags:
- Business Management
- Dynamics NAV
- ERP
- Finance
- Inventory
- Microsoft
- Navision
title: ConfigurationPackage
---
