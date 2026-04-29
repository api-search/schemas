---
description: ''
layout: schema
name: Error
properties_list:
- description: A short description of the error.
  name: title
  type: string
- description: A detailed description of the error.
  name: detail
  type: string
- description: The HTTP status code.
  name: status
  type: integer
provider_name: Microsoft Windows Server
provider_slug: microsoft-windows-server
schema_file: json-schema/iis-administration-error-schema.json
slug: iis-administration-error
source_filename: iis-administration-error-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Error\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"A short description of the error.\"\n    },\n    \"detail\": {\n      \"type\": \"string\",\n      \"description\": \"A detailed description of the error.\"\n    },\n    \"status\": {\n      \"type\": \"integer\",\n      \"description\": \"The HTTP status code.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-windows-server/refs/heads/main/json-schema/iis-administration-error-schema.json
tags:
- Datacenter
- Enterprise
- Infrastructure
- Microsoft
- Operating System
- Server Management
- Windows Server
- Windows Server 2025
title: Error
---
