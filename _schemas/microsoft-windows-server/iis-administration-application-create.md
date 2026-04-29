---
description: Request body for creating a new web application.
layout: schema
name: ApplicationCreate
properties_list:
- description: The virtual path for the application relative to the web site root.
  name: path
  type: string
- description: The physical file system path for the application. The directory must exist.
  name: physical_path
  type: string
- description: The web site that the application should belong to.
  name: website
  type: object
- description: Optional application pool assignment.
  name: application_pool
  type: object
- description: The protocols enabled for this application.
  name: enabled_protocols
  type: string
provider_name: Microsoft Windows Server
provider_slug: microsoft-windows-server
schema_file: json-schema/iis-administration-application-create-schema.json
slug: iis-administration-application-create
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ApplicationCreate\",\n  \"type\": \"object\",\n  \"description\": \"Request body for creating a new web application.\",\n  \"properties\": {\n    \"path\": {\n      \"type\": \"string\",\n      \"description\": \"The virtual path for the application relative to the web site root.\"\n    },\n    \"physical_path\": {\n      \"type\": \"string\",\n      \"description\": \"The physical file system path for the application. The directory must exist.\"\n    },\n    \"website\": {\n      \"type\": \"object\",\n      \"description\": \"The web site that the application should belong to.\"\n    },\n    \"application_pool\": {\n      \"type\": \"object\",\n      \"description\": \"Optional application pool assignment.\"\n    },\n    \"enabled_protocols\": {\n      \"type\": \"string\",\n      \"description\": \"The protocols enabled for this application.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-windows-server/refs/heads/main/json-schema/iis-administration-application-create-schema.json
tags:
- Datacenter
- Enterprise
- Infrastructure
- Microsoft
- Operating System
- Server Management
- Windows Server
- Windows Server 2025
title: ApplicationCreate
---
