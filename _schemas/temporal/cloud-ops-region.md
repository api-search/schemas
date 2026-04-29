---
description: ''
layout: schema
name: Region
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: cloudProvider
  type: string
- description: ''
  name: location
  type: string
provider_name: Temporal
provider_slug: temporal
schema_file: json-schema/cloud-ops-region-schema.json
slug: cloud-ops-region
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Region\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"cloudProvider\": {\n      \"type\": \"string\"\n    },\n    \"location\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/temporal/refs/heads/main/json-schema/cloud-ops-region-schema.json
tags:
- ProCode_API_Composition
- Workflows
title: Region
---
