---
description: Information about the authenticated session
layout: schema
name: SessionInfo
properties_list:
- description: Authenticated user principal name
  name: user
  type: string
- description: Time when the session was created
  name: created_time
  type: string
- description: Time when the session was last accessed
  name: last_accessed_time
  type: string
provider_name: VMware
provider_slug: vmware
schema_file: json-schema/vmware-vsphere-session-info-schema.json
slug: vmware-vsphere-session-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SessionInfo\",\n  \"type\": \"object\",\n  \"description\": \"Information about the authenticated session\",\n  \"properties\": {\n    \"user\": {\n      \"type\": \"string\",\n      \"description\": \"Authenticated user principal name\"\n    },\n    \"created_time\": {\n      \"type\": \"string\",\n      \"description\": \"Time when the session was created\"\n    },\n    \"last_accessed_time\": {\n      \"type\": \"string\",\n      \"description\": \"Time when the session was last accessed\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/json-schema/vmware-vsphere-session-info-schema.json
tags:
- Cloud Computing
- Container Management
- Hybrid Cloud
- Infrastructure
- Virtualization
title: SessionInfo
---
