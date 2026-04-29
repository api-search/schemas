---
description: An issue resolution.
layout: schema
name: Resolution
properties_list:
- description: ''
  name: self
  type: string
- description: ''
  name: id
  type: string
- description: The name of the resolution (e.g., Fixed, Won't Fix, Duplicate).
  name: name
  type: string
- description: ''
  name: description
  type: string
provider_name: Jira
provider_slug: jira
schema_file: json-schema/jira-cloud-platform-rest-resolution-schema.json
slug: jira-cloud-platform-rest-resolution
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Resolution\",\n  \"type\": \"object\",\n  \"description\": \"An issue resolution.\",\n  \"properties\": {\n    \"self\": {\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the resolution (e.g., Fixed, Won't Fix, Duplicate).\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/jira/refs/heads/main/json-schema/jira-cloud-platform-rest-resolution-schema.json
tags:
- Agile
- Issue Tracking
- ITSM
- Project Management
- Service Management
title: Resolution
---
