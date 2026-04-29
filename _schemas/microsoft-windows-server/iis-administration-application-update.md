---
description: Request body for updating a web application. Only include properties that should be changed.
layout: schema
name: ApplicationUpdate
properties_list:
- description: The virtual path for the application.
  name: path
  type: string
- description: The physical file system path for the application.
  name: physical_path
  type: string
- description: ''
  name: application_pool
  type: object
- description: ''
  name: enabled_protocols
  type: string
provider_name: Microsoft Windows Server
provider_slug: microsoft-windows-server
schema_file: json-schema/iis-administration-application-update-schema.json
slug: iis-administration-application-update
source_filename: iis-administration-application-update-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ApplicationUpdate\",\n  \"type\": \"object\",\n  \"description\": \"Request body for updating a web application. Only include properties that should be changed.\",\n  \"properties\": {\n    \"path\": {\n      \"type\": \"string\",\n      \"description\": \"The virtual path for the application.\"\n    },\n    \"physical_path\": {\n      \"type\": \"string\",\n      \"description\": \"The physical file system path for the application.\"\n    },\n    \"application_pool\": {\n      \"type\": \"object\"\n    },\n    \"enabled_protocols\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-windows-server/refs/heads/main/json-schema/iis-administration-application-update-schema.json
tags:
- Datacenter
- Enterprise
- Infrastructure
- Microsoft
- Operating System
- Server Management
- Windows Server
- Windows Server 2025
title: ApplicationUpdate
---
