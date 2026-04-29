---
description: A complete IIS web application resource. Applications belong to a single web site and handle requests at a specific virtual path.
layout: schema
name: Application
properties_list:
- description: The full location path combining the web site name and application path.
  name: location
  type: string
- description: The virtual path of the application relative to the web site root.
  name: path
  type: string
- description: The unique identifier of the application.
  name: id
  type: string
- description: The physical file system path for the application.
  name: physical_path
  type: string
- description: The protocols enabled for this application, as a comma-separated list.
  name: enabled_protocols
  type: string
provider_name: Microsoft Windows Server
provider_slug: microsoft-windows-server
schema_file: json-schema/iis-administration-application-schema.json
slug: iis-administration-application
source_filename: iis-administration-application-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Application\",\n  \"type\": \"object\",\n  \"description\": \"A complete IIS web application resource. Applications belong to a single web site and handle requests at a specific virtual path.\",\n  \"properties\": {\n    \"location\": {\n      \"type\": \"string\",\n      \"description\": \"The full location path combining the web site name and application path.\"\n    },\n    \"path\": {\n      \"type\": \"string\",\n      \"description\": \"The virtual path of the application relative to the web site root.\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the application.\"\n    },\n    \"physical_path\": {\n      \"type\": \"string\",\n      \"description\": \"The physical file system path for the application.\"\n    },\n    \"enabled_protocols\": {\n      \"type\": \"string\",\n      \"description\": \"The protocols enabled for this\
  \ application, as a comma-separated list.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-windows-server/refs/heads/main/json-schema/iis-administration-application-schema.json
tags:
- Datacenter
- Enterprise
- Infrastructure
- Microsoft
- Operating System
- Server Management
- Windows Server
- Windows Server 2025
title: Application
---
