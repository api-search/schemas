---
description: ''
layout: schema
name: AppInstallRequest
properties_list:
- description: Version to install
  name: targetVersion
  type: string
- description: Whether to allow preview versions
  name: allowPreviewVersion
  type: boolean
- description: Whether the ISV EULA is accepted
  name: acceptIsvEula
  type: boolean
- description: Whether to also update dependent apps
  name: allowDependencyUpdate
  type: boolean
provider_name: Microsoft Dynamics NAV
provider_slug: navision
schema_file: json-schema/admin-center-app-install-request-schema.json
slug: admin-center-app-install-request
source_filename: admin-center-app-install-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AppInstallRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"targetVersion\": {\n      \"type\": \"string\",\n      \"description\": \"Version to install\"\n    },\n    \"allowPreviewVersion\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to allow preview versions\"\n    },\n    \"acceptIsvEula\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the ISV EULA is accepted\"\n    },\n    \"allowDependencyUpdate\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to also update dependent apps\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/navision/refs/heads/main/json-schema/admin-center-app-install-request-schema.json
tags:
- Business Management
- Dynamics NAV
- ERP
- Finance
- Inventory
- Microsoft
- Navision
title: AppInstallRequest
---
