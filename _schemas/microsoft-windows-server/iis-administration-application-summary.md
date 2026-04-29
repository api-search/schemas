---
description: A summary representation of an application in list responses.
layout: schema
name: ApplicationSummary
properties_list:
- description: The full location path.
  name: location
  type: string
- description: The virtual path of the application.
  name: path
  type: string
- description: The unique identifier of the application.
  name: id
  type: string
- description: ''
  name: _links
  type: object
provider_name: Microsoft Windows Server
provider_slug: microsoft-windows-server
schema_file: json-schema/iis-administration-application-summary-schema.json
slug: iis-administration-application-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ApplicationSummary\",\n  \"type\": \"object\",\n  \"description\": \"A summary representation of an application in list responses.\",\n  \"properties\": {\n    \"location\": {\n      \"type\": \"string\",\n      \"description\": \"The full location path.\"\n    },\n    \"path\": {\n      \"type\": \"string\",\n      \"description\": \"The virtual path of the application.\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the application.\"\n    },\n    \"_links\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-windows-server/refs/heads/main/json-schema/iis-administration-application-summary-schema.json
tags:
- Datacenter
- Enterprise
- Infrastructure
- Microsoft
- Operating System
- Server Management
- Windows Server
- Windows Server 2025
title: ApplicationSummary
---
