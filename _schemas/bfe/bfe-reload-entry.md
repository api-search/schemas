---
description: A configuration reload entry.
layout: schema
name: ReloadEntry
properties_list:
- description: Unique name of the reload entry.
  name: name
  type: string
- description: Human-readable description of what is reloaded.
  name: description
  type: string
provider_name: BFE
provider_slug: bfe
schema_file: json-schema/bfe-reload-entry-schema.json
slug: bfe-reload-entry
source_filename: bfe-reload-entry-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bfe/refs/heads/main/json-schema/bfe-reload-entry-schema.json\",\n  \"title\": \"ReloadEntry\",\n  \"description\": \"A configuration reload entry.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Unique name of the reload entry.\",\n      \"example\": \"server_data_conf\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable description of what is reloaded.\",\n      \"example\": \"Server data configuration\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bfe/refs/heads/main/json-schema/bfe-reload-entry-schema.json
tags:
- Load Balancer
- Networking
- Open Source
- Traffic Management
- CNCF
- Baidu
title: ReloadEntry
---
