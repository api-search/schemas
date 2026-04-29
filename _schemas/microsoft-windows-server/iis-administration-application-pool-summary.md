---
description: A summary representation of an application pool in list responses.
layout: schema
name: ApplicationPoolSummary
properties_list:
- description: The name of the application pool.
  name: name
  type: string
- description: The unique identifier of the application pool.
  name: id
  type: string
- description: The current status of the application pool.
  name: status
  type: string
- description: ''
  name: _links
  type: object
provider_name: Microsoft Windows Server
provider_slug: microsoft-windows-server
schema_file: json-schema/iis-administration-application-pool-summary-schema.json
slug: iis-administration-application-pool-summary
source_filename: iis-administration-application-pool-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ApplicationPoolSummary\",\n  \"type\": \"object\",\n  \"description\": \"A summary representation of an application pool in list responses.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the application pool.\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the application pool.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the application pool.\"\n    },\n    \"_links\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-windows-server/refs/heads/main/json-schema/iis-administration-application-pool-summary-schema.json
tags:
- Datacenter
- Enterprise
- Infrastructure
- Microsoft
- Operating System
- Server Management
- Windows Server
- Windows Server 2025
title: ApplicationPoolSummary
---
