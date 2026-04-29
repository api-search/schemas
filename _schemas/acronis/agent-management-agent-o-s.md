---
description: Operating system information for an agent
layout: schema
name: AgentOS
properties_list:
- description: ''
  name: family
  type: string
- description: ''
  name: arch
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: version
  type: string
provider_name: Acronis
provider_slug: acronis
schema_file: json-schema/agent-management-agent-o-s-schema.json
slug: agent-management-agent-o-s
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/acronis/refs/heads/main/json-schema/agent-management-agent-o-s-schema.json\",\n  \"title\": \"AgentOS\",\n  \"description\": \"Operating system information for an agent\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"family\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"WINDOWS\",\n        \"LINUX\",\n        \"MACOSX\",\n        \"SOLARIS\"\n      ],\n      \"example\": \"WINDOWS\"\n    },\n    \"arch\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"X86\",\n        \"X64\",\n        \"ARM\",\n        \"ARM64\"\n      ],\n      \"example\": \"X64\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"Windows 11 Pro\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"example\": \"10.0.22621\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acronis/refs/heads/main/json-schema/agent-management-agent-o-s-schema.json
tags:
- Cybersecurity
- Data Protection
- Endpoint Management
title: AgentOS
---
